<template>
  <svg width="24" height="24" fill="none" xmlns="http://www.w3.org/2000/svg" id="mdi-cloud-search-outline" viewBox="0 0 24 24"><linearGradient
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
    </radialGradient><path :fill="fill" :fill-opacity="opacity" d="M15.5,12C18,12 20,14 20,16.5C20,17.38 19.75,18.21 19.31,18.9L22.39,22L21,23.39L17.88,20.32C17.19,20.75 16.37,21 15.5,21C13,21 11,19 11,16.5C11,14 13,12 15.5,12M15.5,14A2.5,2.5 0 0,0 13,16.5A2.5,2.5 0 0,0 15.5,19A2.5,2.5 0 0,0 18,16.5A2.5,2.5 0 0,0 15.5,14M22,13A3,3 0 0,0 19,10H17.5V9.5A5.5,5.5 0 0,0 12,4C9.5,4 7.37,5.69 6.71,8H6A4,4 0 0,0 2,12A4,4 0 0,0 6,16H9V16.5C9,17 9.06,17.5 9.17,18H6A6,6 0 0,1 0,12C0,8.9 2.34,6.36 5.35,6.04C6.6,3.64 9.11,2 12,2C15.64,2 18.67,4.59 19.36,8.04C21.95,8.22 24,10.36 24,13C24,14.65 23.21,16.1 22,17V16.5C22,15.77 21.88,15.06 21.65,14.4C21.87,14 22,13.5 22,13Z" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js";

export default {
  name: 'MaterialIconOutlinedCloudSearch',
  mixins: [icon]
};
</script>