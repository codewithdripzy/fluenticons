<template>
  <svg width="24" height="24" fill="none" xmlns="http://www.w3.org/2000/svg" id="mdi-heart-off-outline" viewBox="0 0 24 24"><linearGradient
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
    </radialGradient><path :fill="fill" :fill-opacity="opacity" d="M2.39 1.73L1.11 3L3.19 5.08C2.45 6 2 7.19 2 8.5C2 12.27 5.4 15.36 10.55 20.03L12 21.35L13.45 20.03C14.32 19.24 15.14 18.5 15.9 17.79L20 22L21.27 20.73M12.1 18.55L12 18.65L11.89 18.55C7.14 14.24 4 11.39 4 8.5C4 7.74 4.22 7.06 4.61 6.5L14.5 16.37C13.74 17.06 12.95 17.78 12.1 18.55M8.3 5.1L6.33 3.13C6.7 3.05 7.1 3 7.5 3C9.24 3 10.91 3.81 12 5.08C13.09 3.81 14.76 3 16.5 3C19.58 3 22 5.41 22 8.5C22 10.84 20.69 12.92 18.47 15.27L17.06 13.86C18.91 11.88 20 10.2 20 8.5C20 6.5 18.5 5 16.5 5C15.1 5 13.74 5.83 13.11 7H10.89C10.38 6.06 9.39 5.34 8.3 5.1Z" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js";

export default {
  name: 'MaterialIconOutlinedHeartOff',
  mixins: [icon]
};
</script>