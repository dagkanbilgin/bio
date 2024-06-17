<template>
  <div class="white-version home-classic spybody">
    <main
      class="main-page-wrapper spybody"
      data-spy="scroll"
      data-target=".navbar-example2"
      data-offset="150"
    >
      <HeadersHeader4 :navItems="navItemsFitnessInstractor" />
      <HerosHero6 />
      <AboutsAbout4 />
      <ServicesService1 />
      <div class="bg-image-area-fitness attachment bg_image--10 bg_image"></div>
      <PortfoliosPortfolio5 />
      <ClientsClients2 :isWhiteMode="true" />
      <TestimonialsTestimonials2 />
      <PricingPricing2 />
      <BlogsBlogs1 />
      <ContactsContact1 />
    </main>
    <FootersFooter2 />
    <CommonComponents />
  </div>
</template>

<script setup>
useSeoMeta({
  title:
    "Home Instractor Fitness White Version || Inbio - Personal Portfolio Vue3 Nuxtjs Template",
  description: "Inbio - Personal Portfolio Vue3 Nuxtjs Template",
});
import { navItemsFitnessInstractor } from "~/data/menu";
</script>

<style lang="scss" scoped></style>
