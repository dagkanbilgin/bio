<template>
  <div class="marketer-features rn-section-gap scrollSpysection" id="about">
    <div class="heading2">
      <div class="container row align-items-end">
        <div class="subtitle col-lg-3 col-sm-12 mb-sm-5">> motto</div>
        <div class="title col-lg-9 col-sm-12">
          my systems approach is about traffic and conversion.
        </div>
      </div>
    </div>
    <div class="marketer-feature g-5 row">
      <div class="col-lg-6 col-md-12">
        <div class="imgContainer">
          <Swiper
            :autoplay="{
              delay: 4000,
            }"
            effect="fade"
            :modules="[Autoplay, EffectFade]"
          >
            <SwiperSlide
              ><nuxt-img
                src="/assets/images/marketer/gallery-44.jpg"
                alt="image"
              />
            </SwiperSlide>
            <SwiperSlide
              ><nuxt-img
                src="/assets/images/marketer/gallery-45.jpg"
                alt="image"
              />
            </SwiperSlide>
          </Swiper>
        </div>
      </div>
      <div class="col-lg-6 col-md-12 col-sm-12 textContainer">
        Every part of my creative and systematic work is built on a strong
        foundation of experience dolor sit amet. Suspendisse varius enim in eros
        elementum tristique. Duis cursus, mi quis viverra ornare, eros dolor
        interdum nulla.
      </div>
    </div>
    <div class="heading2">
      <div class="container row align-items-end">
        <div
          class="subtitle col-lg-3 col-sm-12 mb-0 mb-sm-5 order-2 order-sm-1"
        >
          > method
        </div>
        <div class="title col-lg-9 col-sm-12 order-2 order-sm-1">
          I build websites that convert visitors using design with target clear
          messaging.
        </div>
      </div>
    </div>
    <div class="marketer-feature g-5 row">
      <div class="col-lg-6 col-md-12 col-sm-12 order-2 order-sm-1">
        <div class="imgContainer">
          <Swiper
            :autoplay="{
              delay: 4000,
            }"
            effect="fade"
            :modules="[Autoplay, EffectFade]"
          >
            <SwiperSlide
              ><nuxt-img
                src="/assets/images/marketer/gallery-46.jpg"
                alt="image"
              />
            </SwiperSlide>
            <SwiperSlide
              ><nuxt-img
                src="/assets/images/marketer/gallery-47.jpg"
                alt="image"
              />
            </SwiperSlide>
          </Swiper>
        </div>
      </div>
      <div class="col-lg-6 col-md-12 col-sm-12 textContainer order-1">
        Ensure your business attracts and retains customers. Eros elementum
        tristique varius. To the most part, the interdum is nulla, eros dolor
        autemur.
      </div>
    </div>
  </div>
</template>

<script setup>
import { Autoplay, EffectFade } from "swiper/modules";
import { Swiper, SwiperSlide } from "swiper/vue";
</script>

<style lang="scss" scoped></style>
