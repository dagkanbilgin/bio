<template>
  <div class="template-color-1 home-classic spybody">
    <main
      class="main-page-wrapper spybody"
      data-spy="scroll"
      data-bs-target=".navbar-example2"
      data-offset="150"
    >
      <HeadersHeader9 :navItems="navItemsMarketer" />

      <HerosHero17 />
      <FeaturesFeatures8 />
      <SkillsSkills7 />
      <div class="heading2 mb--100">
        <div class="container row align-items-end">
          <div class="subtitle col-lg-3 col-sm-12 order-2">> goal</div>
          <div class="title col-lg-9 col-sm-12 order-2">
            I help my clients generate traffic, money, and profits.
          </div>
        </div>
      </div>
      <PortfoliosPortfolio11 />
      <PricingPricing2 />
      <TestimonialsTestimonials2 />
      <ContactsContact7 />
    </main>
    <FootersFooter1 />
    <CommonComponents />
  </div>
</template>

<script setup>
useSeoMeta({
  title: "Home Marketer || Inbio - Personal Portfolio Vue3 Nuxtjs Template",
  description: "Inbio - Personal Portfolio Vue3 Nuxtjs Template",
});

import { navItemsMarketer } from "~/data/menu";
</script>

<style lang="scss" scoped></style>
