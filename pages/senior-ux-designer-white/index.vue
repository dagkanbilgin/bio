<template>
  <div class="white-version spybody">
    <Header1 :navItems="navItemsSrDesihner" />
    <div class="main-page-wrapper">
      <HerosHero14 />
      <AboutsAbout9 :isWhiteMode="true" />
      <ClientsClient6 />
      <PortfoliosPortfolio8 />
      <SkillsSkills3 />
      <BannersBanner2 :isWhiteMode="true" />
      <SkillsSkills4 />
      <TestimonialsTestimonials1 />
      <BlogsBlogs1 />
    </div>
    <FootersFooter2 />
    <CommonComponents />
  </div>
</template>

<script setup>
useSeoMeta({
  title:
    "Home Sr Designer White Version || Inbio - Personal Portfolio Vue3 Nuxtjs Template",
  description: "Inbio - Personal Portfolio Vue3 Nuxtjs Template",
});
import Header1 from "~/components/headers/Header1.vue";
import { navItemsSrDesihner } from "~/data/menu";
</script>
