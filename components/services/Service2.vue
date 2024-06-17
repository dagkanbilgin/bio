<template>
  <div
    data-aos="fade-left"
    data-aos-duration="500"
    data-aos-delay="200"
    data-aos-once="true"
    class="rn-skill-area single-card-sticky section-height scrollSpysection"
    id="service"
  >
    <div class="inner">
      <h5 class="title">My Services</h5>
      <ul class="card-list">
        <li v-for="(elm, i) in services2" :key="i">
          <a href="#">{{ elm.text }} <i data-feather="arrow-right"></i></a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script setup>
import { services2 } from "~/data/services";
</script>

<style lang="scss" scoped></style>
