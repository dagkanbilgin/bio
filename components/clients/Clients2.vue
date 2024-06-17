<template>
  <div
    id="client"
    class="rn-client-area rn-client-style-2 rn-section-gap section-separator scrollSpysection"
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
            <span class="subtitle">VISIT MY CLIENT</span>
            <h2 class="title">My Trusted Client</h2>
          </div>
          <div class="skill-style-1">
            <div class="client-card">
              <!-- Start Single Brand  -->
              <div
                v-for="(elm, i) in clients"
                :key="i"
                data-aos="fade-up"
                data-aos-duration="500"
                data-aos-delay="100"
                data-aos-once="true"
                class="main-content"
              >
                <div class="inner text-center">
                  <div class="thumbnail">
                    <a href="#"
                      ><img
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
              <!-- End Single Brand  -->

              <!-- End Single Brand  -->
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { clients } from "~/data/clients";
defineProps(["isWhiteMode"]);
</script>

<style lang="scss" scoped></style>
