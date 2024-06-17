<template>
  <div
    class="rn-testimonial-area rn-section-gap section-separator scrollSpysection"
    id="testimonial"
  >
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <div class="section-title text-center">
            <span class="subtitle">What Clients Say</span>
            <h2 class="title">Testimonial</h2>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-lg-12">
          <div class="testimonial-activation testimonial-pb mb--30">
            <Swiper
              :modules="[Pagination, Navigation]"
              :loop="true"
              :navigation="{
                prevEl: '.snbp1',
                nextEl: '.snbn1',
              }"
              :pagination="{
                el: '.sp1',
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
              <SwiperSlide
                v-for="(elm, i) in testimonials1"
                :key="i"
                class="testimonial mt--50 mt_md--40 mt_sm--40"
              >
                <div class="inner">
                  <div class="card-info">
                    <div class="card-thumbnail">
                      <nuxt-img :src="elm.imageSrc" alt="Testimonial-image" />
                    </div>
                    <div class="card-content">
                      <span class="subtitle mt--10">Rainbow-Themes</span>
                      <h3 class="title">Nevine Acotanza</h3>
                      <span class="designation">Chief Operating Officer</span>
                    </div>
                  </div>
                  <div class="card-description">
                    <div class="title-area">
                      <div class="title-info">
                        <h3 class="title">Android App Development</h3>
                        <span class="date"
                          >via Upwork - Mar 4, 2015 - Aug 30, 2021</span
                        >
                      </div>
                      <div class="rating">
                        <nuxt-img
                          src="/assets/images/icons/rating.png"
                          alt="rating-image"
                        />
                        <nuxt-img
                          src="/assets/images/icons/rating.png"
                          alt="rating-image"
                        />
                        <nuxt-img
                          src="/assets/images/icons/rating.png"
                          alt="rating-image"
                        />
                        <nuxt-img
                          src="/assets/images/icons/rating.png"
                          alt="rating-image"
                        />
                        <nuxt-img
                          src="/assets/images/icons/rating.png"
                          alt="rating-image"
                        />
                      </div>
                    </div>
                    <div class="seperator"></div>
                    <p class="discription">
                      Maecenas finibus nec sem ut imperdiet. Ut tincidunt est ac
                      dolor aliquam sodales. Phasellus sed mauris hendrerit,
                      laoreet sem in, lobortis mauris hendrerit ante. Ut
                      tincidunt est ac dolor aliquam sodales phasellus smauris .
                    </p>
                  </div>
                </div>
              </SwiperSlide></Swiper
            >
            <button class="slide-arrow prev-arrow slick-arrow snbp1" style="">
              <i class="feather-arrow-left"></i>
            </button>
            <button class="slide-arrow next-arrow slick-arrow snbn1" style="">
              <i class="feather-arrow-right"></i>
            </button>
            <ul class="slick-dots sp1" style="" role="tablist"></ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { Pagination, Navigation } from "swiper/modules";
import { Swiper, SwiperSlide } from "swiper/vue";
import { testimonials1 } from "~/data/testimonials";
</script>

<style lang="scss" scoped></style>
