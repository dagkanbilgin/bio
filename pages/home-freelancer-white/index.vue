<template>
  <div class="white-version home-sticky spybody">
    <main class="main-page-wrapper">
      <div class="rn-slider-area">
        <div class="container">
          <div class="row row--30 pt--100 pt_sm--50">
            <div class="col-lg-6"><AboutsAbout5 /></div>
            <div class="col-lg-6">
              <div class="sticky-home-wrapper">
                <AboutsAbout6 />
                <Skill1 />
                <ServicesService2 />
                <PortfoliosPortfolio7 />
                <BlogsBlogs3 />
                <TestimonialsTestimonials3 />
                <ContactsContact4 />
              </div>
            </div>
          </div>
        </div>
      </div>
    </main>
    <CommonComponents />
  </div>
</template>

<script setup>
useSeoMeta({
  title:
    "Home Freelancer White Version || Inbio - Personal Portfolio Vue3 Nuxtjs Template",
  description: "Inbio - Personal Portfolio Vue3 Nuxtjs Template",
});
import Skill1 from "~/components/skills/Skill1.vue";
</script>

<style lang="scss" scoped></style>
