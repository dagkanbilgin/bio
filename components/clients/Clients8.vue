<template>
  <div class="pb--80 pb_md--50 pt--50 section-separator">
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <div
            data-aos="fade-up"
            data-aos-duration="500"
            data-aos-delay="100"
            data-aos-once="true"
            class="section-title"
          >
            <h2 class="title">Brand Carousel</h2>
          </div>

          <div
            class="client-card testimonial-activation-item-3 slick-arrow-style-one mb--60 slick-initialized slick-slider slick-dotted aos-init aos-animate"
          >
            <Swiper
              :loop="true"
              :modules="[Navigation, Pagination]"
              :breakpoints="swiperResponsive"
              :slides-per-view="2"
              :navigation="{ prevEl: '.snbp2', nextEl: '.snbn2' }"
              class="skill-style-1 pb--100"
              :pagination="{
                el: '.sp2',
                bulletActiveClass: 'slick-active',
                clickable: true,

                renderBullet: function (index, className) {
                  return `<li class='${className}' role='presentation'>
                <button
                 
                >
             
                </button>
              </li>`;
                },
              }"
            >
              <SwiperSlide v-for="(elm, i) in clients" :key="i">
                <div
                  data-aos="fade-up"
                  data-aos-duration="500"
                  data-aos-delay="100"
                  data-aos-once="true"
                  class="main-content"
                >
                  <div class="inner text-center">
                    <div class="thumbnail">
                      <a href="#"
                        ><nuxt-img
                          :src="isWhiteMode ? elm.imageDark : elm.image"
                          alt="Client-image"
                      /></a>
                    </div>
                    <div class="seperator"></div>
                    <div class="client-name">
                      <span
                        ><a href="#">{{ elm.name }}</a></span
                      >
                    </div>
                  </div>
                </div>
              </SwiperSlide></Swiper
            >
            <ul class="slick-dots sp2" style="" role="tablist"></ul>
            <button class="slide-arrow prev-arrow slick-arrow snbp2" style="">
              <i class="feather-arrow-left"></i>
            </button>
            <button class="slide-arrow next-arrow slick-arrow snbn2" style="">
              <i class="feather-arrow-right"></i>
            </button>
            <!-- Start Single Brand  -->

            <!-- End Single Brand  -->

            <!-- End Single Brand  -->
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const swiperResponsive = {
  1400: {
    slidesPerView: 4,
    slidesPerGroup: 1,
  },
  1124: {
    slidesPerView: 3,
    slidesPerGroup: 1,
  },
  868: {
    slidesPerView: 2,
    slidesPerGroup: 1,
  },
  576: {
    slidesPerView: 2,
    slidesPerGroup: 1,
  },
};
import { Navigation, Pagination } from "swiper/modules";
import { Swiper, SwiperSlide } from "swiper/vue";
import { clients } from "~/data/clients";
defineProps(["isWhiteMode"]);
</script>

<style lang="scss" scoped></style>
