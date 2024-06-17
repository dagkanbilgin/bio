<template>
  <div id="home" class="rn-slider-area scrollSpysection">
    <!-- Start Single Slide -->
    <div class="slide slider-style-4 bg_image bg_image-doctor">
      <div class="container">
        <div class="row">
          <div class="order-2 order-lg-1 col-lg-9 col-xl-7">
            <div class="content">
              <div class="inner" style="margin-bottom: 0px">
                <span class="subtitle">CONSULTANT EYE SERGEON</span>
                <h1 class="title">
                  Hi, I’m <span>William Lina</span><br />
                  a <span class="span is-visible-one"></span>
                </h1>
                <div>
                  <p class="description">
                    Explore the professional journey, expertise, and
                    achievements of a dedicated medical practitioner. Discover
                    education, experience, clinical skills, research, and
                    patient care .
                  </p>
                  <p></p>
                </div>
                <a
                  class="rn-btn shadow-none"
                  target="_blank"
                  href="https://themeforest.net/checkout/from_item/33188244?license=regular"
                  ><span>Make an Appointment</span></a
                >
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- End Single Slide -->
  </div>
</template>

<script setup>
import Typed from "typed.js";
const typeitInstance = ref();

onMounted(() => {
  typeitInstance.value = new Typed(".is-visible-one", {
    strings: ["  Eye Consultant.", "  Eye Sergeon Specialist."],
    typeSpeed: 26,
    backSpeed: 20,
    startDelay: 200,

    loop: Infinity,
    showCursor: false,
  });
});
onUnmounted(() => {
  typeitInstance.value?.destroy();
});
</script>

<style lang="scss" scoped></style>
