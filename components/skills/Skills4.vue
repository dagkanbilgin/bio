<template>
  <div class="rn-section-gap scrollSpysection" id="tool">
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <div
            data-aos="fade-up"
            data-aos-duration="300"
            data-aos-delay="100"
            data-aos-once="true"
            class="section-title text-center"
          >
            <span class="subtitle">SOFTWARE</span>
            <h2 class="title">Tools I use</h2>
          </div>
        </div>
      </div>
      <div class="rn-skill-area">
        <div
          class="inner slide text-center"
          style="padding-bottom: 0px !important"
        >
          <div class="skill-share-inner pt--50">
            <span class="title">Primary Skills on</span>
            <ul
              class="skill-share d-flex liststyle justify-content-center primary-skills"
              style="max-width: 600px; margin: 0px auto"
            >
              <li v-for="(elm, i) in primarySkills" :key="i">
                <nuxt-img :src="elm.src" alt="Icons Images" />
              </li>
            </ul>
          </div>
          <div class="skill-share-inner skill-share-inner-width pt--100">
            <span class="title">Secondary Skills on</span>
            <ul
              class="skill-share d-flex liststyle justify-content-center"
              style="max-width: 600px; margin: 0px auto"
            >
              <li v-for="(elm, i) in secondarySkills" :key="i">
                <nuxt-img :src="elm.src" alt="Icons Images" />
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { primarySkills, secondarySkills } from "~/data/skills";
</script>

<style lang="scss" scoped></style>
