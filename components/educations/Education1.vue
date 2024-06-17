<template>
  <div
    id="educations"
    class="rn-education-area rn-section-gap section-separator scrollSpysection"
  >
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
            <span class="subtitle">Phd, Master and Bachelo</span>
            <h2 class="title">Education</h2>
          </div>
        </div>
      </div>
      <div class="row mt--10">
        <div class="col-12 mt_experience">
          <!-- single skills -->
          <div
            v-for="(elm, i) in education"
            :key="i"
            data-aos="fade-up"
            data-aos-duration="500"
            data-aos-delay="100"
            data-aos-once="true"
            class="experience-style-two"
          >
            <div class="experience-left">
              <div class="experience-image">
                <nuxt-img :src="elm.imageSrc" alt="Personal Portfolio" />
              </div>
              <div class="experience-center">
                <span class="date">{{ elm.date }}</span>
                <h4 class="experience-title">{{ elm.title }}</h4>
                <h6 class="subtitle">{{ elm.subtitle }}</h6>
                <p class="disc">{{ elm.disc }}</p>
              </div>
            </div>
            <div class="experience-right">
              <div class="experience-footer">
                <a class="rn-btn" href="#contacts"><span>CONTACT ME</span></a>
              </div>
            </div>
          </div>
          <!-- single skills -->
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { education } from "~/data/education";
</script>

<style lang="scss" scoped></style>
