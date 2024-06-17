<template>
  <div class="template-color-1 home-sticky">
    <HeadersHeader3 />
    <main class="page-wrapper-two position-relative p-lg-4">
      <HerosHero3 />
      <div style="max-width: 100%; overflow: clip">
        <FeaturesFeatures3 /> <PortfoliosPortfolio1 />
        <ResumesResume1 />
        <ClientsClients1 />
        <PricingPricing1 />
        <BlogsBlogs1 />
        <ContactsContact1 />
      </div>

      <FootersFooter1 />
    </main>
    <CommonComponents />
  </div>
</template>

<script setup>
useSeoMeta({
  title: "Home Consulting || Inbio - Personal Portfolio Vue3 Nuxtjs Template",
  description: "Inbio - Personal Portfolio Vue3 Nuxtjs Template",
});
</script>

<style lang="scss" scoped></style>
