<template>
  <svg width="24" height="24" fill="none" xmlns="http://www.w3.org/2000/svg" id="mdi-notebook-minus" viewBox="0 0 24 24"><linearGradient
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
    </radialGradient><path :fill="fill" :fill-opacity="opacity" d="M3 7V5H5V4C5 2.9 5.9 2 7 2H13V9L15.5 7.5L18 9V2H19C20 2 21 3 21 4V13.8C20.1 13.3 19.1 13 18 13C14.7 13 12 15.7 12 19C12 20.1 12.3 21.1 12.8 22H7C5.9 22 5 21 5 20V19H3V17H5V13H3V11H5V7H3M5 5V7H7V5H5M5 19H7V17H5V19M5 13H7V11H5V13M14 18V20H22V18H14Z" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js";

export default {
  name: 'MaterialIconFilledNotebookMinus',
  mixins: [icon]
};
</script>