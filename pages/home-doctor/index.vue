<template>
  <div class="template-color-1 spybody">
    <HeadersHeader7 :navItems="navItemsDoctor" />
    <div class="main-page-wrapper">
      <HerosHero13 />
      <FeaturesFeatures5 />
      <AboutsAbout8 />
      <FeaturesFeatures6 />
      <TestimonialsTestimonials1 />
      <AppintmentAppointment1 />
      <BlogsBlogs1 />
      <BannersBanner1 />
      <ClientsClients5 />
    </div>
    <FootersFooter2 />
    <CommonComponents />
  </div>
</template>

<script setup>
useSeoMeta({
  title: "Home Doctor || Inbio - Personal Portfolio Vue3 Nuxtjs Template",
  description: "Inbio - Personal Portfolio Vue3 Nuxtjs Template",
});
import { navItemsDoctor } from "~/data/menu";
</script>

<style lang="scss" scoped></style>
