<template>
  <svg width="24" height="24" fill="none" xmlns="http://www.w3.org/2000/svg" id="mdi-panorama-vertical-outline" viewBox="0 0 24 24"><linearGradient
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
    </radialGradient><path :fill="fill" :fill-opacity="opacity" d="M6.54,20C7.31,17.4 7.7,14.72 7.7,12C7.7,9.28 7.31,6.6 6.54,4H17.45C16.68,6.6 16.29,9.28 16.29,12C16.29,14.72 16.68,17.4 17.45,20M19.94,21.12C18.84,18.18 18.3,15.09 18.3,12C18.3,8.91 18.85,5.82 19.94,2.88C20,2.77 20,2.66 20,2.57C20,2.23 19.77,2 19.37,2H4.63C4.23,2 4,2.23 4,2.57C4,2.67 4,2.77 4.06,2.88C5.16,5.82 5.71,8.91 5.71,12C5.71,15.09 5.16,18.18 4.07,21.12C4,21.23 4,21.34 4,21.43C4,21.76 4.23,22 4.63,22H19.38C19.77,22 20,21.76 20,21.43C20,21.33 20,21.23 19.94,21.12Z" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js";

export default {
  name: 'MaterialIconOutlinedPanoramaVertical',
  mixins: [icon]
};
</script>