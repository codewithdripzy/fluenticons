<template>
  <svg width="24" height="24" fill="none" xmlns="http://www.w3.org/2000/svg" id="mdi-calendar-edit-outline" viewBox="0 0 24 24"><linearGradient
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
    </radialGradient><path :fill="fill" :fill-opacity="opacity" d="M21.7 13.35L20.7 14.35L18.65 12.35L19.65 11.35C19.85 11.14 20.19 11.13 20.42 11.35L21.7 12.63C21.89 12.83 21.89 13.15 21.7 13.35M12 18.94V21H14.06L20.12 14.88L18.07 12.88L12 18.94M5 19H10V21H5C3.9 21 3 20.11 3 19V5C3 3.9 3.9 3 5 3H6V1H8V3H16V1H18V3H19C20.11 3 21 3.9 21 5V9H5V19M5 5V7H19V5H5Z" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js";

export default {
  name: 'MaterialIconOutlinedCalendarEdit',
  mixins: [icon]
};
</script>