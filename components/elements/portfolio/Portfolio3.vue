<template>
  <div class="rn-project-area portfolio-style-two rn-section-gap">
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <div
            data-aos="fade-up"
            data-aos-duration="500"
            data-aos-delay="100"
            data-aos-once="true"
            class="section-title text-left mb_md--25 mb_sm--25"
          >
            <h2 class="title">Poftfolio Style Three</h2>
          </div>
        </div>
      </div>
      <div
        data-aos="fade-up"
        data-aos-duration="1000"
        data-aos-delay="300"
        data-aos-once="true"
        id="carouselExampleControls"
        class="carousel slide"
        data-ride="carousel"
      >
        <div class="carousel-inner">
          <!-- Start Single Item  -->

          <div
            v-for="(elm, i) in portfolios2"
            :key="i"
            :class="`carousel-item ${!i ? 'active' : ''}`"
          >
            <div class="portfolio-single">
              <div class="row direction">
                <div class="col-lg-5">
                  <div class="inner">
                    <h5 class="title">{{ elm.title }}</h5>
                    <p class="discription">
                      {{ elm.description }}
                    </p>
                    <div class="ft-area">
                      <div class="feature-wrapper">
                        <div
                          v-for="(elm2, i2) in elm.features"
                          :key="i2"
                          class="single-feature"
                        >
                          <i data-feather="check"></i>
                          <p>{{ elm2 }}</p>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="col-lg-7 col-xl-7">
                  <div class="thumbnail">
                    <nuxt-img
                      :width="800"
                      :height="600"
                      :src="elm.imgSrc"
                      alt="image"
                    />
                  </div>
                </div>
              </div>
            </div>
          </div>
          <!-- End Single Item  -->
        </div>
        <button
          class="carousel-control-prev"
          role="button"
          data-bs-target="#carouselExampleControls"
          data-bs-slide="prev"
        >
          <i data-feather="chevron-left"></i>
        </button>
        <button
          class="carousel-control-next"
          role="button"
          data-bs-target="#carouselExampleControls"
          data-bs-slide="next"
        >
          <i data-feather="chevron-right"></i>
        </button>
      </div>
    </div>
  </div>
</template>

<script setup>
import { portfolios2 } from "~/data/portfolios";
</script>

<style lang="scss" scoped></style>
