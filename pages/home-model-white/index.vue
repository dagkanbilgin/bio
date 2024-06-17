<template>
  <div class="white-version home-classic spybody">
    <main
      class="main-page-wrapper spybody"
      data-spy="scroll"
      data-bs-target=".navbar-example2"
      data-offset="150"
    >
      <HeadersHeader10 :navItems="navItemsModel" />

      <Hero2 />
      <FeaturesFeatures2 />
      <AboutsAbout2 />
      <div class="bg-image-area-fitness attachment bg_image--8 bg_image"></div>
      <PortfoliosPortfolio3 />
      <ClientsClients2 :isWhiteMode="true" />
      <ContactsContact1 />
    </main>
    <FootersFooter1 />
    <CommonComponents />
  </div>
</template>

<script setup>
useSeoMeta({
  title:
    "Home Model White Version || Inbio - Personal Portfolio Vue3 Nuxtjs Template",
  description: "Inbio - Personal Portfolio Vue3 Nuxtjs Template",
});
import Hero2 from "~/components/Heros/Hero2.vue";
import { navItemsModel } from "~/data/menu";
</script>

<style lang="scss" scoped></style>
