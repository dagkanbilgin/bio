<template>
  <div style="position: absolute; height: 100vh; left: 0; right: 0">
    <NuxtParticles
      id="tsparticles"
      :options="options"
      @load="onLoad"
    ></NuxtParticles>
  </div>

  <section
    id="home"
    class="slider-style-5 rn-section-gap pb--110 align-items-center with-particles scrollSpysection mw-100"
  >
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <div class="banner-inner">
            <div class="thumbnail gradient-border gradient-animation">
              <nuxt-img
                :width="500"
                :height="500"
                id="border"
                class="gradient-border"
                src="/assets/images/slider/banner-06.png"
                alt="image"
              />
            </div>
            <h1>Al-Amin Bali</h1>
            <!-- type headline start-->
            <span class="cd-headline clip is-full-width">
              <span>I am a</span>
              <!-- ROTATING TEXT -->

              <b class="is-visible is-visible-one ml--10 pt--5"></b>
            </span>
            <!-- type headline end -->
            <div class="button-area">
              <a class="rn-btn" href="#contacts"><span>CONTACT ME</span></a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const props = defineProps(["isWhiteMode"]);
import Typed from "typed.js";
const typeitInstance = ref();
const options = {
  backgroundMode: {
    enable: true,
    zIndex: -1,
  },
  fullScreen: {
    enable: false,
    zIndex: -1,
  },
  fpsLimit: 70,
  particles: {
    number: { value: 50, density: { enable: !0, value_area: 800 } },
    color: { value: props.isWhiteMode ? "#000" : "#fff" },
    shape: {
      type: "circle",
      stroke: { width: 0, color: "#ff0000" },
      polygon: { nb_sides: 5 },
      image: { src: "", width: 100, height: 100 },
    },
    opacity: {
      value: { min: 0.3, max: 1 },
      random: !1,
      anim: { enable: !1, speed: 2, opacity_min: 0, sync: !1 },
    },
    size: {
      value: { min: 1, max: 5 },
      random: !1,
      anim: { enable: 1, speed: 20, size_min: 0, sync: !1 },
    },
    line_linked: {
      enable: !0,
      distance: 100,
      color: "#fff",
      opacity: { min: 0.5, max: 1 },
      width: 1,
    },
    move: {
      enable: !0,
      speed: 2,
      direction: "none",
      random: !1,
      straight: !1,
      out_mode: "out",
      bounce: !1,
      attract: { enable: !1, rotateX: 3e3, rotateY: 3e3 },
    },
    array: [],
  },
  interactivity: {
    detect_on: "canvas",
    events: {
      onhover: { enable: !0, mode: "grab" },
      onclick: { enable: !0, mode: "push" },
      resize: !0,
    },
    modes: {
      grab: { distance: 100, line_linked: { opacity: 1 } },
      bubble: { distance: 200, size: 80, duration: 0.4 },
      repulse: { distance: 200, duration: 0.4 },
      push: { particles_nb: 4 },
      remove: { particles_nb: 2 },
    },
    mouse: {},
  },

  detectRetina: true,
};
const onLoad = (container) => {
  // Do something with the container
  container.pause();
  setTimeout(() => container.play(), 2000);
};
onMounted(() => {
  typeitInstance.value = new Typed(".is-visible-one", {
    strings: ["  Lawyer.", "  Consulter.", "  Developer."],
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

<style lang="scss">
#tsparticles {
  canvas {
    position: absolute !important;
    // display: none;
  }
}
</style>
