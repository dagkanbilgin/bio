<template>
  <div
    style="padding: 25px; margin: 0px"
    class="white-version box-wrapper spybody"
  >
    <div style="position: relative">
      <HeadersHeader1 :navItems="navItemsInstractor" />
      <main class="main-page-wrapper">
        <HerosHero10 />
        <FeaturesFeatures1 />
        <PortfoliosPortfolio1 />
        <ResumesResume1 />
        <TestimonialsTestimonials1 />
        <ClientsClients1 :isWhiteMode="true" />
        <PricingPricing1 />
        <BlogsBlogs1 />
        <ContactsContact3 />
      </main>
      <FootersFooter1 />
    </div>
    <CommonComponents />
  </div>
</template>

<script setup>
useSeoMeta({
  title:
    "Home Instractor White Version  || Inbio - Personal Portfolio Vue3 Nuxtjs Template",
  description: "Inbio - Personal Portfolio Vue3 Nuxtjs Template",
});
import { navItemsInstractor } from "~/data/menu";
</script>
<style lang="scss" scoped></style>
