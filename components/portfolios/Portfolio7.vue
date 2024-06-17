<template>
  <div
    data-aos="fade-left"
    data-aos-duration="500"
    data-aos-delay="200"
    data-aos-once="true"
    id="portfolio"
    class="rn-portfolio-area single-card-sticky section-height scrollSpysection"
  >
    <div class="inner">
      <h5 class="title">My Portfolio</h5>
      <ul class="card-list">
        <li v-for="(elm, i) in portfolios3" :key="i">
          <a href="#">{{ elm.text }} <i data-feather="arrow-right"></i></a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script setup>
import { portfolios3 } from "~/data/portfolios";
</script>

<style lang="scss" scoped></style>
