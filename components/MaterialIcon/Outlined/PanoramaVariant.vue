<template>
  <svg width="24" height="24" fill="none" xmlns="http://www.w3.org/2000/svg" id="mdi-panorama-variant-outline" viewBox="0 0 24 24"><linearGradient
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
    </radialGradient><path :fill="fill" :fill-opacity="opacity" d="M21 4C20.4 4 17.4 5.5 12 5.5C6.7 5.5 3.5 4 3 4C2.5 4 2 4.4 2 5V19C2 19.6 2.5 20 3 20C3.6 20 6.5 18.5 12 18.5C17.4 18.5 20.4 20 21 20C21.5 20 22 19.6 22 19V5C22 4.4 21.5 4 21 4M20 17.6C18 17 15.4 16.5 12 16.5C8.6 16.5 6 17 4 17.6V6.4C6.6 7.1 9.3 7.5 12 7.5C15.4 7.5 18 7 20 6.4V17.6M9.2 11L5.5 15.4C7.5 15.1 9.7 15 12 15C14.3 15 16.5 15.1 18.5 15.4L14 10L11.2 13.4L9.2 11Z" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js";

export default {
  name: 'MaterialIconOutlinedPanoramaVariant',
  mixins: [icon]
};
</script>