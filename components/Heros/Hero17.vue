<template>
  <div
    id="home"
    class="rn-slider-area scrollSpysection position-relative home-marketer-hero overflow-hidden"
  >
    <!-- Start Single Slide -->
    <div class="slide slider-style-4">
      <div class="container">
        <div class="row justify-content-center text-center">
          <div class="order-2 order-lg-1 col-lg-11 col-xl-10">
            <div class="content">
              <div
                class="inner model mb--0 mt--0 mt_lg--5 mt_md--5 mt_sm--5 text-center"
              >
                <div class="img mb-5">
                  <nuxt-img
                    :width="256"
                    :height="256"
                    src="/assets/images/marketer.jpg"
                    alt="image"
                  />
                </div>
                <h3 class="subtitle">I CAN HELP YOU</h3>
                <h1 class="title">Convert visitors into customers.</h1>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="position-absolute video-container">
      <client-only>
        <iframe
          class="iframe"
          frameborder="0"
          allowfullscreen="true"
          src="https://www.youtube.com/embed/FpAM4fYj-4g?autoplay=1&mute=1&controls=0&showinfo=0&loop=1&rel=0&playlist=FpAM4fYj-4g
"
        ></iframe
      ></client-only>
    </div>
    <div class="bg"></div>
    <!-- End Single Slide -->
  </div>
</template>

<script setup></script>

<style lang="scss">
.video-container {
  pointer-events: none;
  z-index: 15;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;

  mix-blend-mode: multiply;
  iframe {
    height: 110%;
    width: 400vw;
    position: absolute;

    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
}
.bg {
  position: absolute;
  top: 0%;
  width: 100%;
  height: 100%;
  background-image: linear-gradient(270deg, #ff014f 0%, #6a67ce 70%);
}

.content {
  position: relative;
  z-index: 20;
}
.html5-video-container {
  display: none !important;
}
</style>
