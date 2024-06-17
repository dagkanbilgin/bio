<template>
  <div class="template-color-1 spybody">
    <Header1 :navItems="navItemsDesignerTwo" />
    <div class="main-page-wrapper">
      <HerosHero15 />
      <PortfoliosPortfolio9 />
      <PhotographyPhotograpphy />
      <AwardsAward1 />
      <div
        class="bg-image-area-fitness attachment bg_image--15 bg_image mt--60"
      ></div>
      <PricingPricing3 />
      <ClientsClients2 />
      <ContactsContact5 />
    </div>
    <FootersFooter1 />
    <CommonComponents />
  </div>
</template>

<script setup>
useSeoMeta({
  title: "Home Designer Two || Inbio - Personal Portfolio Vue3 Nuxtjs Template",
  description: "Inbio - Personal Portfolio Vue3 Nuxtjs Template",
});
import Header1 from "~/components/headers/Header1.vue";
import { navItemsDesignerTwo } from "~/data/menu";
</script>
