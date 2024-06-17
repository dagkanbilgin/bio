<template>
  <div id="case-studies" class="rn-section-gap pt--0 scrollSpysection">
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <div
            data-aos="fade-up"
            data-aos-duration="500"
            data-aos-delay="100"
            data-aos-once="true"
            class="section-title text-center"
          >
            <span class="subtitle">FEATURES</span>
            <h2 class="title">Case Study</h2>
          </div>
        </div>
      </div>
      <div class="row mt--50">
        <div
          v-for="(elm, i) in caseStudies"
          :key="i"
          class="col-12 mt_experience"
        >
          <!-- single skills -->
          <div
            data-aos="fade-up"
            data-aos-duration="500"
            data-aos-delay="100"
            data-aos-once="true"
            class="case-studies"
          >
            <div class="left">
              <div class="img">
                <nuxt-img
                  :width="379"
                  :height="204"
                  :src="elm.imgSrc"
                  alt="image"
                />
              </div>
              <div class="title">
                {{ elm.title }}
              </div>
            </div>
            <div class="right">
              <div class="desc">
                {{ elm.desc }}
              </div>
              <a href="#" class="arrow-up">
                <i aria-hidden="true" class="rbt feather-arrow-up-right"></i>
              </a>
            </div>
          </div>
          <!-- single skills -->
        </div>
      </div>
    </div>
  </div>
</template>
<script setup>
import { caseStudies } from "~/data/caseStudies";
</script>

<style lang="scss" scoped></style>
