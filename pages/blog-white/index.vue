<template>
  <div class="white-version">
    <HeadersHeader8 />
    <main class="main-page-wrapper">
      <CommonBreadcumb current-page="Blog" />
      <div class="rn-section-gap">
        <BlogsBlogs2 />
      </div>
    </main>
    <CommonComponents />
    <FootersFooter2 />
  </div>
</template>

<script setup>
useSeoMeta({
  title:
    "Blog White Version || Inbio - Personal Portfolio Vue3 Nuxtjs Template",
  description: "Inbio - Personal Portfolio Vue3 Nuxtjs Template",
});
</script>

<style lang="scss" scoped></style>
