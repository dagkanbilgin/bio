<template>
  <div
    class="rn-testimonial-area testimonial-style-2 testimonial-with-carousel rn-section-gapTop pb--80 pb_md--50 section-separator scrollSpysection"
    id="testimonial"
  >
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <div
            data-aos="fade-up"
            data-aos-duration="500"
            data-aos-delay="100"
            data-aos-once="true"
            class="section-title text-center mb--20 mb_md--20 mb_sm--20"
          >
            <span class="subtitle">What Clients Say</span>
            <h2 class="title">Testimonial</h2>
          </div>
        </div>
      </div>

      <div
        class="testimonial-activation-item-3 slick-arrow-style-one mb--60 slick-initialized slick-slider slick-dotted aos-init aos-animate"
        data-aos="fade-up"
        data-aos-duration="500"
        data-aos-delay="300"
        data-aos-once="true"
      >
        <Swiper
          :loop="true"
          :modules="[Navigation, Pagination]"
          :breakpoints="swiperResponsive"
          :navigation="{ prevEl: '.snbp3', nextEl: '.snbn3' }"
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
          <!-- Start single Testimonial -->
          <SwiperSlide
            v-for="(elm, i) in testimonials2"
            :key="i"
            class="rn-testimonial"
          >
            <div class="testimonial-inner">
              <div class="testimonial-header">
                <div class="thumbnail">
                  <nuxt-img :src="elm.imgSrc" alt="client-image" />
                </div>
                <h5 class="ts-header">
                  <span class="text-color-primary">{{ elm.name }}</span>
                  {{ elm.position }}
                </h5>
              </div>
              <div class="testimonial-body">
                <p class="discription">
                  {{ elm.comment }}
                </p>
              </div>
            </div>
          </SwiperSlide>
        </Swiper>
        <ul class="slick-dots sp2" style="" role="tablist"></ul>
        <button class="slide-arrow prev-arrow slick-arrow snbp3" style="">
          <i class="feather-arrow-left"></i>
        </button>
        <button class="slide-arrow next-arrow slick-arrow snbn3" style="">
          <i class="feather-arrow-right"></i>
        </button>
        <!-- End single Testimonial -->
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
import { Navigation, Pagination } from "swiper/modules";
import { Swiper, SwiperSlide } from "swiper/vue";
import { testimonials2 } from "~/data/testimonials";
</script>

<style lang="scss" scoped></style>
