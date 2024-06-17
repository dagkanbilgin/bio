<template>
  <div
    id="pricing"
    class="rn-pricing-area pricing-style-2 rn-section-gap section-separator scrollSpysection"
  >
    <div class="container">
      <div class="row">
        <div
          data-aos="fade-up"
          data-aos-duration="1000"
          data-aos-delay="100"
          data-aos-once="true"
          class="col-lg-4 col-sm-12"
        >
          <div class="title-area-wrapper mb_md--20 mb_sm--20">
            <div class="section-title text-left">
              <span class="subtitle">Pricing</span>
              <h2 class="title">Fitness plane pricing</h2>
            </div>
            <p class="title-disc">
              Use the free templates with your whole team or choose a premium.
              ith your whole team or choose a premium.
            </p>
            <p class="title-disc-2">
              Get the bundle and get lifetime support and one year updates.
            </p>
          </div>
        </div>

        <div
          v-for="(pricing, index) in pricings"
          :key="index"
          :data-aos="pricing.dataAos"
          :class="pricing.wrapperClass"
        >
          <div class="pricing-wrapper">
            <div class="ts-header">
              <h6>{{ pricing.title }}</h6>
              <span>{{ pricing.duration }}</span>
            </div>
            <h3 class="price">{{ pricing.price }}</h3>
            <div class="pricing-body">
              <div
                v-for="(feature, featureIndex) in pricing.features"
                :key="featureIndex"
                class="feature"
              >
                <i
                  :class="{ off: !feature.available }"
                  data-feather="check"
                ></i>
                <span class="name" :class="{ off: !feature.available }">{{
                  feature.name
                }}</span>
              </div>
            </div>
            <div class="pricing-footer">
              <a class="rn-btn" href="#contacts"><span>BUY NOW</span></a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { pricings } from "~/data/pricing";
</script>

<style lang="scss" scoped></style>
