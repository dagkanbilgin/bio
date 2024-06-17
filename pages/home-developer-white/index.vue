<template>
  <div class="white-version spybody">
    <main class="main-page-wrapper">
      <HeadersHeader1 :navItems="navItemsDeveloper" />
      <HerosHero5 />
      <ExperiencesExperience1 />
      <EducationsEducation1 />
      <ResumesResume1 />
      <PortfoliosPortfolio4 />
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
    "Home Developer White Version || Inbio - Personal Portfolio Vue3 Nuxtjs Template",
  description: "Inbio - Personal Portfolio Vue3 Nuxtjs Template",
});
import { navItemsDeveloper } from "~/data/menu";
</script>

<style lang="scss" scoped></style>
