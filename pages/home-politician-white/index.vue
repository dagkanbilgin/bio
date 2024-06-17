<template>
  <div class="white-version home-vedio spybody">
    <HeadersHeader1 :navItems="navItemsPolititian" />
    <main class="main-page-wrapper">
      <HerosHero12 />
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
    <CommonComponents />
  </div>
</template>

<script setup>
useSeoMeta({
  title:
    "Home Polititian White Version || Inbio - Personal Portfolio Vue3 Nuxtjs Template",
  description: "Inbio - Personal Portfolio Vue3 Nuxtjs Template",
});
import { navItemsPolititian } from "~/data/menu";
</script>
<style lang="scss" scoped></style>
