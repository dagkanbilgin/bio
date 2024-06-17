<template>
  <div
    data-aos="fade-left"
    data-aos-duration="500"
    data-aos-delay="200"
    data-aos-once="true"
    id="blog"
    class="rn-blog-area single-card-sticky section-height scrollSpysection"
  >
    <div class="inner">
      <h5 class="title">My Blog</h5>
      <ul class="card-list">
        <li v-for="(elm, i) in blogs2" :key="i">
          <a href="#">{{ elm.title }}<i data-feather="arrow-right"></i></a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script setup>
import { blogs2 } from "~/data/blogs";
</script>

<style lang="scss" scoped></style>
