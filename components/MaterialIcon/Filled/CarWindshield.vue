<template>
  <svg width="24" height="24" fill="none" xmlns="http://www.w3.org/2000/svg" id="mdi-car-windshield" viewBox="0 0 24 24"><linearGradient
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
    </radialGradient><path :fill="fill" :fill-opacity="opacity" d="M22.63 15.5L20.21 5.85A1 1 0 0 0 19.14 5.1C17.8 5.24 14.14 5.5 12 5.5S6.2 5.24 4.86 5.1A1 1 0 0 0 3.79 5.85L1.37 15.5A1.5 1.5 0 0 0 2.55 17.36A61.5 61.5 0 0 0 12 18A61.5 61.5 0 0 0 21.45 17.36A1.5 1.5 0 0 0 22.63 15.5Z" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js";

export default {
  name: 'MaterialIconFilledCarWindshield',
  mixins: [icon]
};
</script>