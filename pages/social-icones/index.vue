<template>
  <div class="template-color-1">
    <HeadersHeader8 />
    <main class="main-page-wrapper">
      <CommonBreadcumb current-page="Social Icons" />
      <Social1 />
      <Social2 />
      <Social3 />
    </main>
    <CommonComponents />

    <FootersFooter2 />
  </div>
</template>

<script setup>
useSeoMeta({
  title: "Social Icon || Inbio - Personal Portfolio Vue3 Nuxtjs Template",
  description: "Inbio - Personal Portfolio Vue3 Nuxtjs Template",
});
import Social1 from "../../components/elements/socials/Social1.vue";
import Social2 from "../../components/elements/socials/Social2.vue";
import Social3 from "../../components/elements/socials/Social3.vue";
</script>

<style lang="scss" scoped></style>
