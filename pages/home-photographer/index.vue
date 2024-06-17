<template>
  <div class="template-color-1 home-classic spybody">
    <main class="main-page-wrapper spybody">
      <HeadersHeader6 :navItems="navItemsPhotographar" />
      <HerosHero11 />
      <AboutsAbout7 />
      <SkillsSkills2 />
      <FeaturesFeatures4 />
      <div class="section-separator"></div>
      <PortfoliosPortfolio5 />
      <div class="section-separator"></div>
      <ClientsClients2 />
      <TestimonialsTestimonials2 />
      <PricingPricing3 />
      <BlogsBlogs1 />
      <ContactsContact1 />
    </main>
    <FootersFooter1 />
    <CommonComponents />
  </div>
</template>

<script setup>
useSeoMeta({
  title: "Home Photographer || Inbio - Personal Portfolio Vue3 Nuxtjs Template",
  description: "Inbio - Personal Portfolio Vue3 Nuxtjs Template",
});
import { navItemsPhotographar } from "~/data/menu";
</script>

<style lang="scss" scoped></style>
