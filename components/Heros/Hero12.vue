<template>
  <div class="rn-slider-area scrollSpysection" id="home">
    <!-- Start Slider Area -->
    <div class="rn-slider-area">
      <div class="slide slider-style-2">
        <div class="container">
          <div class="row row--30">
            <div class="order-2 order-lg-1 col-lg-7 mt_md--40 mt_sm--40">
              <div class="content">
                <div class="inner">
                  <span class="subtitle">Welcome to my world</span>
                  <h1 class="title">
                    Hi, I’m <span>Zara Fatima</span><br /><span class="span">
                      Social Politician.</span
                    >
                  </h1>
                  <div>
                    <p class="description">
                      I use animation as a third dimension by which to simplify
                      experiences and kuiding thro each and every interaction.
                      I’m not adding motion just to spruce things up, but doing
                      it in ways that.
                    </p>
                  </div>
                </div>
                <div class="row">
                  <div class="col-lg-6 col-xl-6 col-md-6 col-sm-6 col-12">
                    <div class="social-share-inner-left">
                      <span class="title">find with me</span>
                      <ul class="social-share d-flex liststyle">
                        <li
                          v-for="(elm, i) in socials.slice(0, 3)"
                          :key="i"
                          class=""
                        >
                          <a :href="elm.link"
                            ><i :data-feather="elm.icon"></i
                          ></a>
                        </li>
                      </ul>
                    </div>
                  </div>
                  <div
                    class="col-lg-6 col-xl-6 col-md-6 col-sm-6 col-12 mt_mobile--30"
                  >
                    <div class="skill-share-inner">
                      <span class="title">best skill on</span>
                      <ul class="skill-share d-flex liststyle">
                        <li v-for="(elm, i) in skillsHero" :key="i">
                          <nuxt-img :src="elm.src" alt="Icons Images" />
                        </li>
                      </ul>
                    </div>
                  </div>
                </div>
              </div>
            </div>

            <div class="order-1 order-lg-2 col-lg-5">
              <div
                id="carouselExampleControls w-100"
                class="carousel slide"
                data-ride="carousel"
              >
                <Swiper
                  :modules="[Navigation]"
                  :navigation="{
                    prevEl: '.snbph1',
                    nextEl: '.snbnh1',
                  }"
                  :slides-per-view="1"
                  style="width: 100%; overflow: hidden"
                >
                  <SwiperSlide
                    v-for="(elm, i) in images"
                    :key="i"
                    class="swiper-slide"
                  >
                    <img
                      class="w-100 modal-portfolio-image"
                      :src="elm"
                      alt="portfolio-large-05"
                    />
                  </SwiperSlide>
                </Swiper>

                <a
                  class="carousel-control-prev snbph1"
                  role="button"
                  data-slide="prev"
                >
                  <span class="" aria-hidden="true">
                    <i data-feather="chevron-left"></i>
                  </span>
                  <span class="sr-only">Previous</span>
                </a>
                <a
                  class="carousel-control-next snbnh1"
                  role="button"
                  data-slide="next"
                >
                  <span class="" aria-hidden="true">
                    <i data-feather="chevron-right"></i>
                  </span>
                  <span class="sr-only">Next</span>
                </a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- End Slider Area -->
  </div>
</template>

<script setup>
import { skillsHero } from "~/data/skills";
import { socials } from "~/data/socials";
const images = [
  "/assets/images/slider/banner-07.png",
  "/assets/images/slider/banner-08.png",
];
import { Navigation } from "swiper/modules";
import { SwiperSlide } from "swiper/vue";
import { Swiper } from "swiper/vue";
</script>

<style lang="scss" scoped></style>
