<template>
  <svg width="24" height="24" fill="none" xmlns="http://www.w3.org/2000/svg" id="mdi-phone-missed" viewBox="0 0 24 24"><linearGradient
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
    </radialGradient><path :fill="fill" :fill-opacity="opacity" d="M23.71,16.67C20.66,13.77 16.54,12 12,12C7.46,12 3.34,13.77 0.29,16.67C0.11,16.85 0,17.1 0,17.38C0,17.65 0.11,17.9 0.29,18.08L2.77,20.56C2.95,20.74 3.2,20.86 3.5,20.86C3.75,20.86 4,20.75 4.18,20.57C4.97,19.83 5.86,19.21 6.84,18.72C7.17,18.56 7.4,18.22 7.4,17.82V14.72C8.85,14.25 10.39,14 12,14C13.6,14 15.15,14.25 16.6,14.72V17.82C16.6,18.22 16.83,18.56 17.16,18.72C18.14,19.21 19.03,19.83 19.82,20.57C20,20.75 20.25,20.86 20.5,20.86C20.8,20.86 21.05,20.74 21.23,20.56L23.71,18.08C23.89,17.9 24,17.65 24,17.38C24,17.1 23.89,16.85 23.71,16.67M6.5,5.5L12,11L19,4L18,3L12,9L7.5,4.5H11V3H5V9H6.5V5.5Z" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js";

export default {
  name: 'MaterialIconFilledPhoneMissed',
  mixins: [icon]
};
</script>