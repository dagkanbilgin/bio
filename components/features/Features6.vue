<template>
  <div
    class="rn-service-area rn-section-gap section-separator scrollSpysection"
    id="services"
  >
    <div class="container">
      <div class="row justify-content-center">
        <div class="col-lg-6 col-md-12">
          <div
            class="section-title text-center"
            data-aos="fade-up"
            data-aos-duration="500"
            data-aos-delay="100"
            data-aos-once="true"
          >
            <span class="subtitle">SERVICES</span>
            <h2 class="title">Services For You & Your Family</h2>
          </div>
        </div>
      </div>
      <div class="row row--25 mt_md--10 mt_sm--10">
        <!-- Start Single Service -->
        <div
          v-for="(elm, i) in features2"
          :key="i"
          data-aos="fade-up"
          data-aos-duration="500"
          data-aos-delay="100"
          data-aos-once="true"
          class="col-lg-6 col-xl-4 col-md-6 col-sm-12 col-12 mt--50 mt_md--30 mt_sm--30"
        >
          <div class="rn-service">
            <div class="inner">
              <div class="icon">
                <i :data-feather="elm.icon"></i>
              </div>
              <div class="content">
                <h4 class="title">
                  <a href="#">{{ elm.title }}</a>
                </h4>
                <p class="description">
                  {{ elm.description }}
                </p>
                <a class="read-more-button" href="#"
                  ><i class="feather-arrow-right"></i
                ></a>
              </div>
            </div>
            <a class="over-link" href="#"></a>
          </div>
        </div>

        <!-- End SIngle Service -->
      </div>
    </div>
  </div>
</template>

<script setup>
import { features2 } from "~/data/features";
</script>

<style lang="scss" scoped></style>
