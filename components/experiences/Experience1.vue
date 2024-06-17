<template>
  <div
    id="experiences"
    class="rn-experience-area section-separator rn-section-gap scrollSpysection"
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
            <span class="subtitle">Over 10 years of experience</span>
            <h2 class="title">My Experience</h2>
          </div>
        </div>
      </div>
      <div class="row mt--10">
        <div class="col-12 mt_experience">
          <!-- single skills -->
          <div
            v-for="(elm, i) in experience"
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
import { experience } from "~/data/experience";
</script>

<style lang="scss" scoped></style>
