<template>
  <svg width="24" height="24" fill="none" xmlns="http://www.w3.org/2000/svg" id="mdi-content-save-off" viewBox="0 0 24 24"><linearGradient
      v-if="fill === 'url(#g1)'"
      id="g1"
      :gradientTransform="'rotate(' + angle + ')'"
    >
      <stop class="main-stop" offset="0%" :stop-color="start" />
      <stop class="alt-stop" offset="100%" :stop-color="end" />
    </linearGradient>
    <radialGradient
      v-if="fill === 'url(#g2)'"
      id="g2"
      cx="50%"
      cy="50%"
      r="50%"
    >
      <stop :stop-color="start" offset="0%" />
      <stop :stop-color="end" offset="100%" />
    </radialGradient><path :fill="fill" :fill-opacity="opacity" d="M8.2 5L6.2 3H17L21 7V17.8L12.2 9H15V5H8.2M22.11 21.46L20.84 22.73L19.1 21C19.07 21 19.03 21 19 21H5C3.9 21 3 20.11 3 19V5C3 4.97 3 4.93 3 4.9L1.11 3L2.39 1.73L22.11 21.46M7.11 9L5 6.89V9H7.11M14.89 16.78L11.22 13.11C9.95 13.46 9 14.61 9 16C9 17.66 10.34 19 12 19C13.39 19 14.54 18.05 14.89 16.78Z" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js";

export default {
  name: 'MaterialIconFilledContentSaveOff',
  mixins: [icon]
};
</script>