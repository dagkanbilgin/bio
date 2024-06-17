<template>
  <div class="white-version">
    <HeadersHeader8 />
    <main class="main-page-wrapper">
      <CommonBreadcumb current-page="Popup Video" />
      <VideoPopup1 />
      <VideoPopup2 />
      <VideoPopup3 />
    </main>

    <FootersFooter2 />
  </div>
</template>

<script setup>
useSeoMeta({
  title:
    "Video Popup White Version || Inbio - Personal Portfolio Vue3 Nuxtjs Template",
  description: "Inbio - Personal Portfolio Vue3 Nuxtjs Template",
});
import VideoPopup1 from "~/components/elements/videoPopup/VideoPopup1.vue";
import VideoPopup2 from "~/components/elements/videoPopup/VideoPopup2.vue";
import VideoPopup3 from "~/components/elements/videoPopup/VideoPopup3.vue";
</script>

<style lang="scss" scoped></style>
