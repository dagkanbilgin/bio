<template>
  <div class="white-version spybody">
    <div style="position: relative">
      <HeadersHeader1 :navItems="navItemsLawyer" />
      <main class="main-page-wrapper">
        <HerosHero16 :isWhiteMode="true" />
        <BannersBanner3 />
        <FeaturesFeatures7 />
        <EducationsCaseStudies />
        <BannersBanner4 />
        <AwardsAwards2 />
        <TestimonialsTestimonials1 />
        <Lawers />
        <ContactsContact6 :isWhiteMode="true" />
        <BlogsBlogs1 />
      </main>
      <FootersFooter2 />
    </div>
    <CommonComponents />
  </div>
</template>

<script setup>
useSeoMeta({
  title:
    "Home Lawyer White Version || Inbio - Personal Portfolio Vue3 Nuxtjs Template",
  description: "Inbio - Personal Portfolio Vue3 Nuxtjs Template",
});
import Lawers from "~/components/lawers/Lawers.vue";
import { navItemsLawyer } from "~/data/menu";
</script>
<style lang="scss" scoped></style>
