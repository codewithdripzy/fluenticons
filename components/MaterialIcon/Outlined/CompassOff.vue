<template>
  <svg width="24" height="24" fill="none" xmlns="http://www.w3.org/2000/svg" id="mdi-compass-off-outline" viewBox="0 0 24 24"><linearGradient
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
    </radialGradient><path :fill="fill" :fill-opacity="opacity" d="M1,3.5L2.28,2.25L21.75,21.72L20.5,23L17.7,20.22C16.08,21.34 14.12,22 12,22A10,10 0 0,1 2,12C2,9.88 2.66,7.92 3.78,6.3L1,3.5M7,17L9.39,11.91L5.23,7.74C4.45,9 4,10.44 4,12A8,8 0 0,0 12,20C13.56,20 15,19.55 16.26,18.77L12.09,14.61L7,17M17,7L14.62,12.05L11.95,9.38L17,7M12,2A10,10 0 0,1 22,12C22,14.1 21.35,16.06 20.24,17.67L18.8,16.22C19.56,15 20,13.55 20,12A8,8 0 0,0 12,4C10.45,4 9,4.44 7.78,5.2L6.33,3.76C7.94,2.65 9.9,2 12,2Z" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js";

export default {
  name: 'MaterialIconOutlinedCompassOff',
  mixins: [icon]
};
</script>