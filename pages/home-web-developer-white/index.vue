<template>
  <div class="white-version home-sticky spybody">
    <HeadersHeader5 />
    <main class="page-wrapper-two p-lg-4">
      <HerosHero7 />
      <div style="max-width: 100%; overflow: clip">
        <FeaturesFeatures3 />
        <PortfoliosPortfolio6 />
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
    "Home Web Developer White Version || Inbio - Personal Portfolio Vue3 Nuxtjs Template",
  description: "Inbio - Personal Portfolio Vue3 Nuxtjs Template",
});
</script>

<style lang="scss" scoped></style>
