<template>
  <svg width="24" height="24" fill="none" xmlns="http://www.w3.org/2000/svg" id="mdi-movie-edit" viewBox="0 0 24 24"><linearGradient
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
    </radialGradient><path :fill="fill" :fill-opacity="opacity" d="M21.04 11.13C20.9 11.13 20.76 11.19 20.65 11.3L19.65 12.3L21.7 14.35L22.7 13.35C22.92 13.14 22.92 12.79 22.7 12.58L21.42 11.3C21.31 11.19 21.18 11.13 21.04 11.13M19.07 12.88L13 18.94V21H15.06L21.12 14.93L19.07 12.88M11 20H3C1.9 20 1 19.11 1 18V6C1 4.89 1.9 4 3 4H4L6 8H9L7 4H9L11 8H14L12 4H14L16 8H19L17 4H21V8.12L11 18.11V20Z" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js";

export default {
  name: 'MaterialIconFilledMovieEdit',
  mixins: [icon]
};
</script>