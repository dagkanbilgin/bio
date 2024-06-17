<template>
  <div
    class="rn-video-popup-area rn-section-gapBottom bg_color--1 line-separator"
  >
    <div class="container">
      <div class="row">
        <!-- Start Single Video Button  -->
        <div class="col-lg-6 col-md-6 col-12">
          <div class="thumbnail position-relative">
            <nuxt-img
              class="w-100"
              src="/assets/images/portfolio/portfolio-06.jpg"
              alt="About Images"
            />
            <a
              @click="videoPopupActive = true"
              id="play-video"
              class="video-play-button cursor-pointer"
            >
              <span></span>
            </a>
          </div>
        </div>
        <!-- End Single Video Button  -->

        <!-- Start Single Video Button  -->
        <div class="col-lg-6 col-md-6 col-12 mt_sm--30">
          <div class="thumbnail position-relative">
            <nuxt-img
              class="w-100"
              src="/assets/images/portfolio/portfolio-05.jpg"
              alt="About Images"
            />

            <a
              @click="videoPopupActive = true"
              class="video-play-button play-video cursor-pointer"
            >
              <span></span>
            </a>
            <div class="video-overlay video-overlay">
              <a class="video-overlay-close">×</a>
            </div>
          </div>
        </div>
        <!-- End Single Video Button  -->
      </div>
    </div>
  </div>
  <div
    @click="videoPopupActive = false"
    :class="`video-overlay ${videoPopupActive ? 'open' : ''}`"
  >
    <a @click="videoPopupActive = false" class="video-overlay-close">×</a>
    <iframe
      v-if="videoPopupActive"
      width="80%"
      height="80%"
      src="https://www.youtube.com/embed/7e90gBu4pas"
      frameborder="0"
      allowfullscreen
    ></iframe>
  </div>
</template>

<script setup>
const videoPopupActive = ref(false);
</script>

<style lang="scss" scoped></style>
