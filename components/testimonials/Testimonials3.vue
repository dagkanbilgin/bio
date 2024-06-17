<template>
  <div
    data-aos="fade-left"
    data-aos-duration="500"
    data-aos-delay="200"
    data-aos-once="true"
    id="testimonial"
    class="rn-testimonial-area testimonial-style-2 section-height scrollSpysection"
  >
    <div class="inner">
      <h5 class="title">Testimonial</h5>

      <!-- carousel area Start -->

      <div
        class="rn-testimonial-carousel testimonial-item-one rn-slick-dot-style dot-position-left slick-arrow-style-one arrow-top-align slick-initialized slick-slider slick-dotted"
        data-aos="fade-up"
        data-aos-duration="500"
        data-aos-delay="300"
        data-aos-once="true"
      >
        <Swiper
          :loop="true"
          :modules="[Navigation, Pagination]"
          :slides-per-view="1"
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
          <SwiperSlide v-for="(elm, i) in testimonials2" :key="i">
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
        <button
          class="slide-arrow prev-arrow slick-arrow snbp3"
          style="top: -28%"
        >
          <i class="feather-arrow-left"></i>
        </button>
        <button
          class="slide-arrow next-arrow slick-arrow snbn3"
          style="top: -28%"
        >
          <i class="feather-arrow-right"></i>
        </button>
        <!-- End single Testimonial -->
      </div>
      <!-- carousel area End -->
    </div>
  </div>
</template>

<script setup>
import { Navigation, Pagination } from "swiper/modules";
import { Swiper, SwiperSlide } from "swiper/vue";
import { testimonials2 } from "~/data/testimonials";
</script>

<style lang="scss" scoped></style>
