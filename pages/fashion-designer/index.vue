<template>
  <div class="template-color-1 home-classic spybody">
    <main
      class="main-page-wrapper spybody"
      data-spy="scroll"
      data-target=".navbar-example2"
      data-offset="150"
    >
      <HeadersHeader10 :navItems="navItemsFashionDesigner" />
      <HerosHero4 />
      <AboutsAbout3 />
      <PortfoliosPortfolio1 />
      <ClientsClients2 />
      <TestimonialsTestimonials1 />
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
    "Home Fashion Designer || Inbio - Personal Portfolio Vue3 Nuxtjs Template",
  description: "Inbio - Personal Portfolio Vue3 Nuxtjs Template",
});
import { navItemsFashionDesigner } from "~/data/menu";
</script>

<style lang="scss" scoped></style>
