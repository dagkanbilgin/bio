<template>
  <div
    style="margin: 0px"
    class="template-color-1 box-wrapper spybody home-box-wrapper"
  >
    <div style="position: relative">
      <HeadersHeader1 :navItems="navItemsInstractor" />
      <main class="main-page-wrapper">
        <HerosHero10 />
        <FeaturesFeatures1 />
        <PortfoliosPortfolio1 />
        <ResumesResume1 />
        <TestimonialsTestimonials1 />
        <ClientsClients1 />
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
  title: "Home Instractor || Inbio - Personal Portfolio Vue3 Nuxtjs Template",
  description: "Inbio - Personal Portfolio Vue3 Nuxtjs Template",
});
import { navItemsInstractor } from "~/data/menu";
</script>
<style lang="scss" scoped></style>
