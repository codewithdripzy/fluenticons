<template>
  <svg width="24" height="24" fill="none" xmlns="http://www.w3.org/2000/svg" id="mdi-briefcase-edit" viewBox="0 0 24 24"><linearGradient
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
    </radialGradient><path :fill="fill" :fill-opacity="opacity" d="M14,2A2,2 0 0,1 16,4V6H20A2,2 0 0,1 22,8L10.85,19C10.85,20.1 10.85,19.5 10.85,21H4C2.89,21 2,20.1 2,19V8C2,6.89 2.89,6 4,6H8V4C8,2.89 8.89,2 10,2H14M14,6V4H10V6H14M21.04,12.13C20.9,12.13 20.76,12.19 20.65,12.3L19.65,13.3L21.7,15.35L22.7,14.35C22.92,14.14 22.92,13.79 22.7,13.58L21.42,12.3C21.31,12.19 21.18,12.13 21.04,12.13M19.07,13.88L13,19.94V22H15.06L21.12,15.93L19.07,13.88Z" /></svg>
</template>

<script>
import icon from "../../../mixins/icon.js";

export default {
  name: 'MaterialIconFilledBriefcaseEdit',
  mixins: [icon]
};
</script>