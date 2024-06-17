<template>
  <div class="rn-video-popup-area rn-section-gap bg_color--1 line-separator">
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <div class="thumbnail position-relative">
            <nuxt-img
              class="w-100"
              src="/assets/images/portfolio/portfolio-11.jpg"
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
