<template>
  <div class="template-color-1">
    <HeadersHeader8 />
    <main class="main-page-wrapper">
      <CommonBreadcumb current-page="Portfolio" />
      <ElementsPortfolioPortfolio1 />
      <ElementsPortfolioPortfolio2 />
      <ElementsPortfolioPortfolio3 />
    </main>
    <CommonComponents />

    <FootersFooter2 />
  </div>
</template>

<script setup>
useSeoMeta({
  title: "Portfolio || Inbio - Personal Portfolio Vue3 Nuxtjs Template",
  description: "Inbio - Personal Portfolio Vue3 Nuxtjs Template",
});
</script>

<style lang="scss" scoped></style>
