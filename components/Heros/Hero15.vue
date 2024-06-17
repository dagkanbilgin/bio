<template>
  <div id="home" class="rn-slider-area scrollSpysection">
    <div class="slide slider-style-1 slider-sr-designer">
      <div class="container position-relative hero-senior-designer">
        <div class="designer2-image">
          <nuxt-img
            :width="663"
            :height="673"
            src="/assets/images/slider/banner12.png"
            alt="image"
          />
        </div>
        <div
          class="texts position-absolute"
          style="
            display: flex;
            width: 100%;
            /* justify-content: center; */
            align-items: center;
            flex-direction: column;
            margin-top: 50px;
          "
        >
          <div class="text-1">👋 my name is Inbio & I am a freelance</div>
          <div class="text-2">Webdesigner</div>
          <div class="text-3">& Photographer</div>
          <div class="text-4">based in Nevada, USA ❤️</div>
        </div>
        <div class="client-img">
          <nuxt-img
            :width="500"
            :height="100"
            src="/assets/images/client/client-logos.png"
            alt="image"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped></style>
