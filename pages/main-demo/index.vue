<template>
  <div class="template-color-1 spybody">
    <Header1 :navItems="navItemsMainDemo" />
    <div class="main-page-wrapper">
      <HerosHero1 />
      <FeaturesFeatures1 />
      <PortfoliosPortfolio1 />
      <ResumesResume1 />
      <TestimonialsTestimonials1 />
      <ClientsClients1 />
      <PricingPricing1 />
      <BlogsBlogs1 />
      <ContactsContact1 />
    </div>
    <FootersFooter2 />
    <CommonComponents />
  </div>
</template>

<script setup>
useSeoMeta({
  title: "Home Main Demo || Inbio - Personal Portfolio Vue3 Nuxtjs Template",
  description: "Inbio - Personal Portfolio Vue3 Nuxtjs Template",
});
import Header1 from "~/components/headers/Header1.vue";
import { navItemsMainDemo } from "~/data/menu";
</script>
