<template>
  <div class="rn-portfolio-area rn-section-gap scrollSpysection" id="portfolio">
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <div class="section-title text-center">
            <span class="subtitle"
              >Visit my portfolio and keep your feedback</span
            >
            <h2 class="title">My Portfolio</h2>
          </div>
        </div>
      </div>

      <div class="row mt--10 mt_md--10 mt_sm--10">
        <!-- Start Single Portfolio -->
        <div
          v-for="(elm, i) in photograph"
          :key="i"
          data-aos="fade-up"
          data-aos-delay="100"
          data-aos-once="true"
          class="col-lg-6 col-xl-6 col-md-6 col-12 mt--30 mt_md--30 mt_sm--30"
        >
          <div
            class="rn-portfolio w-100"
            @click="currentPortfolioModal = elm"
            data-bs-toggle="modal"
            data-bs-target="#portfolioModal3"
          >
            <div class="inner w-100">
              <div class="thumbnail w-100">
                <a class="w-100" href="javascript:void(0)">
                  <nuxt-img
                    class="w-100"
                    :width="800"
                    :height="600"
                    :src="elm.imgSrc"
                    alt="Personal Portfolio Images"
                  />
                </a>
              </div>
              <div class="content">
                <div class="category-info">
                  <div class="category-list">
                    <a href="javascript:void(0)">{{ elm.category }}</a>
                  </div>
                  <div class="meta">
                    <span
                      ><a href="javascript:void(0)"
                        ><i class="feather-heart"></i
                      ></a>
                      {{ elm.likes }}</span
                    >
                  </div>
                </div>
                <h4 class="title">
                  <a href="javascript:void(0)"
                    >{{ elm.title }} <i class="feather-arrow-up-right"></i
                  ></a>
                </h4>
              </div>
            </div>
          </div>
        </div>
        <!-- End Single Portfolio -->
      </div>
    </div>
  </div>
</template>

<script setup>
import { currentPortfolioModal } from "~/context/modalContent";
import { photograph } from "~/data/photograph";
</script>

<style lang="scss" scoped></style>
