<template>
  <div class="container scrollSpysection" id="portfolio">
    <div class="row">
      <div class="col-lg-12">
        <div class="section-title text-center">
          <span class="subtitle"
            >HERE IS A SAMPLE OF PROJECTS I'VE WORKED ON.</span
          >
          <h2 class="title">Selected projects</h2>
        </div>
      </div>
    </div>
    <div
      v-for="(item, index) in portfolioItems"
      :key="index"
      class="box-area-1 mt--40 sr-designer-portfolio"
      style="width: 100%; padding: 0; overflow: hidden"
    >
      <div class="row">
        <div
          class="col-lg-6 content"
          :style="{
            padding: '7%',
            backgroundImage: item.backgroundImage,
          }"
        >
          <div class="title-area">
            <span>{{ item.title }}</span>
            <h4 class="title mt--20 mt-sm-2">{{ item.subtitle }}</h4>
          </div>
          <div class="description mb--15">
            <p>{{ item.description }}</p>
          </div>
          <div class="section-separator mt--20"></div>
          <div
            class="mt--16 mt-sm-2 lern-more"
            style="font-size: 16px; padding-top: 40px"
          >
            Learn More About This Case Study
          </div>
        </div>
        <div class="col-lg-6" style="padding: 0px !important">
          <nuxt-img
            style="height: 100%; object-fit: cover; width: 100%"
            :src="item.imageSrc"
            alt="image"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { portfolioItems } from "~/data/portfolios";
</script>

<style lang="scss" scoped></style>
