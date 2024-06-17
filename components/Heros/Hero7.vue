<template>
  <section
    id="home"
    class="slider-style-6 web-developer height--100 rn-section-gap align-items-center with-particles bg_image bg_image--11 scrollSpysection"
    data-black-overlay="5"
  >
    <div id="particles-js"></div>
    <div class="wrapper">
      <div class="container">
        <div class="row">
          <div class="banner-inner text-center">
            <h1 class="fs--100">KRISTINA SMOLYER</h1>
            <!-- type headline start-->
            <span class="cd-headline clip is-full-width">
              <span>I am a</span>
              <!-- ROTATING TEXT -->

              <b class="is-visible is-visible-one ml--10 pt--5"></b>
            </span>
            <!-- type headline end -->
            <div class="button-area">
              <a class="rn-btn shadow-none" href="#contacts"
                ><span>CONTACT ME</span></a
              >
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import Typed from "typed.js";
const typeitInstance = ref();

onMounted(() => {
  typeitInstance.value = new Typed(".is-visible-one", {
    strings: [" Lawyer.", " Consulter.", " Developer."],
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
