<template>
  <div
    class="rn-portfolio-area rn-section-gap section-separator scrollSpysection"
    id="portfolio"
  >
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

      <div class="row row--25 mt--10 mt_md--10 mt_sm--10">
        <!-- Start Single Portfolio -->

        <div
          v-for="(elm, i) in portfolios.slice(0, 3)"
          :key="i"
          data-aos="fade-up"
          data-aos-delay="100"
          data-aos-once="true"
          class="col-lg-6 col-xl-4 col-md-6 col-12 mt--50 mt_md--30 mt_sm--30"
        >
          <div
            class="rn-portfolio"
            data-bs-toggle="modal"
            @click="currentPortfolioModal = elm"
            data-bs-target="#exampleModalCenterportFolio2"
          >
            <div class="inner">
              <div class="thumbnail">
                <a href="javascript:void(0)">
                  <nuxt-img
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
import { portfolios } from "~/data/portfolios";
</script>

<style lang="scss" scoped></style>
