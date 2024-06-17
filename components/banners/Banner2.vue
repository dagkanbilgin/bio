<template>
  <div class="container">
    <div
      style="width: 100%; margin-top: 40px; padding: 0; overflow: hidden"
      class="contact-about-area sr-designer-banner"
    >
      <div class="row">
        <div
          class="col-lg-8 order-2 content"
          style="
            padding: 5%;
            background-image: linear-gradient(45deg, #191829 0%, #212428 100%);
          "
        >
          <div class="title-area">
            <span>E-Learning Platform</span>

            <h4 class="title mt-5">Enhancing Student Success</h4>
          </div>
          <div class="description">
            <p>
              See how our design improvements on an e-learning platform led to
              higher engagement, better retention rates, and improved learning
              outcomes.
            </p>
          </div>
          <div class="section-separator mt-5"></div>
          <div class="mt-5" style="font-size: 16px; padding-top: 40px">
            Learn More About This Case Study
          </div>
        </div>
        <div class="col-lg-4 order-1" style="padding: 0px !important">
          <nuxt-img
            style="height: 100%; object-fit: cover; width: 100%"
            :src="
              isWhiteMode
                ? '/assets/images/man-lv.png'
                : '/assets/images/slider/banner13.png'
            "
            alt="image"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
defineProps(["isWhiteMode"]);
</script>

<style lang="scss" scoped></style>
