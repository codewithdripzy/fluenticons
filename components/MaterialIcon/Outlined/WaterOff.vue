<template>
  <svg width="24" height="24" fill="none" xmlns="http://www.w3.org/2000/svg" id="mdi-water-off-outline" viewBox="0 0 24 24"><linearGradient
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
    </radialGradient><path :fill="fill" :fill-opacity="opacity" d="M22.11 21.46L2.39 1.73L1.11 3L7.65 9.54C6.74 11.03 6 12.65 6 14.23C6 17.54 8.69 20.23 12 20.23C13.74 20.23 15.3 19.5 16.4 18.29L20.84 22.73L22.11 21.46M12 18.23C9.78 18.23 8 16.45 8 14.23C8 13.5 8.5 12.27 9.14 11.03L15 16.88C14.26 17.71 13.2 18.23 12 18.23M11.14 7.94L9.71 6.5C10.57 5.38 11.25 4.61 11.25 4.61L12 3.77L12.75 4.61C12.75 4.61 14.03 6.06 15.32 7.94S18 12.07 18 14.23C18 14.41 18 14.59 17.97 14.77L15.46 12.26C15 11.23 14.37 10.07 13.68 9.07C12.84 7.85 12.44 7.42 12 6.9C11.73 7.21 11.5 7.5 11.14 7.94Z" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js";

export default {
  name: 'MaterialIconOutlinedWaterOff',
  mixins: [icon]
};
</script>