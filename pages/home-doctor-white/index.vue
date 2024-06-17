<template>
  <div class="white-version spybody">
    <HeadersHeader7 :navItems="navItemsDoctor" />
    <div class="main-page-wrapper">
      <HerosHero13 />
      <FeaturesFeatures5 />
      <AboutsAbout8 :isWhiteMode="true" />
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
  title:
    "Home Doctor White Version || Inbio - Personal Portfolio Vue3 Nuxtjs Template",
  description: "Inbio - Personal Portfolio Vue3 Nuxtjs Template",
});
import { navItemsDoctor } from "~/data/menu";
</script>

<style lang="scss" scoped></style>
