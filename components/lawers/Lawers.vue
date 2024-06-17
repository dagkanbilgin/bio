<template>
  <div
    id="consultant"
    class="rn-section-gap section-separator scrollSpysection"
  >
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <div
            class="section-title text-center"
            data-aos="fade-up"
            data-aos-duration="500"
            data-aos-delay="100"
            data-aos-once="true"
          >
            <span class="subtitle">OUR CONSULTANT</span>
            <h2 class="title">Join With Us</h2>
          </div>
        </div>
      </div>
      <div class="team-mambers mt--40">
        <div
          v-for="(member, index) in lawyers"
          :key="index"
          class="team-mamber"
        >
          <div class="img">
            <nuxt-img
              :width="306"
              :height="408"
              :src="member.image"
              alt="image"
            />
          </div>
          <div class="text">
            <div class="name">{{ member.name }}</div>
            <div class="title">{{ member.title }}</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { lawyers } from "~/data/lawers";
</script>

<style lang="scss" scoped></style>
