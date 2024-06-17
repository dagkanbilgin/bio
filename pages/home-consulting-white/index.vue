<template>
  <div class="white-version home-sticky spybody" style="width: 100vw">
    <HeadersHeader3 />
    <main class="page-wrapper-two p-lg-4">
      <HerosHero3 :isWhiteMode="true" />
      <div style="max-width: 100%; overflow: clip">
        <FeaturesFeatures3 />
        <PortfoliosPortfolio1 />
        <ResumesResume1 />
        <ClientsClients1 :isWhiteMode="true" />
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
  title:
    "Home Consulting White Version || Inbio - Personal Portfolio Vue3 Nuxtjs Template",
  description: "Inbio - Personal Portfolio Vue3 Nuxtjs Template",
});
</script>

<style lang="scss" scoped></style>
