<template>
  <svg width="24" height="24" fill="none" xmlns="http://www.w3.org/2000/svg" id="mdi-bed-double-outline" viewBox="0 0 24 24"><linearGradient
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
    </radialGradient><path :fill="fill" :fill-opacity="opacity" d="M8 5C7.5 5 7 5.21 6.61 5.6S6 6.45 6 7V10C5.47 10 5 10.19 4.59 10.59S4 11.47 4 12V17H5.34L6 19H7L7.69 17H16.36L17 19H18L18.66 17H20V12C20 11.47 19.81 11 19.41 10.59S18.53 10 18 10V7C18 6.45 17.8 6 17.39 5.6S16.5 5 16 5M8 7H11V10H8M13 7H16V10H13M6 12H18V15H6Z" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js";

export default {
  name: 'MaterialIconOutlinedBedDouble',
  mixins: [icon]
};
</script>