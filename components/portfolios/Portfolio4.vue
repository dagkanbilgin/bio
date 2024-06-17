<template>
  <div
    id="portfolio"
    class="rn-portfolio-area portfolio-style-three rn-section-gap section-separator scrollSpysection"
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
            <span class="subtitle"
              >Visit my portfolio and keep your feedback</span
            >
            <h2 class="title">My Portfolio</h2>
          </div>
        </div>
      </div>
      <div class="row mt--25 mt_md--5 mt_sm--5">
        <div class="col-lg-12">
          <div
            data-aos="fade-up"
            data-aos-duration="500"
            data-aos-delay="200"
            data-aos-once="true"
            class="portfolio-wrapper portfolio-slick-activation slick-arrow-style-one rn-slick-dot-style slick-slider"
          >
            <!-- Start Single Portfolio  -->
            <Swiper
              :loop="true"
              :modules="[Navigation]"
              :breakpoints="swiperResponsive"
              :navigation="{ prevEl: '.snbp2', nextEl: '.snbn2' }"
            >
              <SwiperSlide
                v-for="(elm, i) in portfolios"
                :key="i"
                class="rn-portfolio-slick"
              >
                <div
                  class="rn-portfolio"
                  @click="currentPortfolioModal = elm"
                  data-bs-toggle="modal"
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
                          <a href="javascript:void(0)">{{
                            elm.category.toLocaleUpperCase()
                          }}</a>
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
                          >{{ elm.title }}<i class="feather-arrow-up-right"></i
                        ></a>
                      </h4>
                    </div>
                  </div>
                </div> </SwiperSlide
            ></Swiper>
            <button class="slide-arrow prev-arrow slick-arrow snbp2" style="">
              <i class="feather-arrow-left"></i>
            </button>
            <button class="slide-arrow next-arrow slick-arrow snbn2" style="">
              <i class="feather-arrow-right"></i>
            </button>
            <!-- End Single Portfolio  -->
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const swiperResponsive = {
  1400: {
    slidesPerView: 3,
    slidesPerGroup: 1,
  },
  1124: {
    slidesPerView: 2,
    slidesPerGroup: 1,
  },
  868: {
    slidesPerView: 1,
    slidesPerGroup: 1,
  },
  576: {
    slidesPerView: 1,
    slidesPerGroup: 1,
  },
};
import { Navigation } from "swiper/modules";
import { Swiper, SwiperSlide } from "swiper/vue";
import { currentPortfolioModal } from "~/context/modalContent";
import { portfolios } from "~/data/portfolios";
</script>

<style lang="scss" scoped></style>
