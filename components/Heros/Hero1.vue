<template>
  <div id="home" class="rn-slider-area scrollSpysection">
    <div class="slide slider-style-1">
      <div class="container">
        <div class="row row--30 align-items-center">
          <div
            class="order-2 order-lg-1 col-lg-7 mt_md--50 mt_sm--50 mt_lg--30"
          >
            <div class="content">
              <div class="inner">
                <span class="subtitle">Welcome to my world</span>
                <h1 class="title">
                  Hi, I’m <span>Jone Lee</span><br />
                  <span class="header-caption" id="page-top">
                    <!-- type headline start-->
                    <span class="cd-headline clip is-full-width">
                      <!-- ROTATING TEXT -->

                      a <b class="is-visible is-visible-one"></b>
                    </span>
                    <!-- type headline end -->
                  </span>
                </h1>

                <div>
                  <p class="description">
                    I use animation as a third dimension by which to simplify
                    experiences and kuiding thro each and every interaction. I’m
                    not adding motion just to spruce things up, but doing it in
                    ways that.
                  </p>
                </div>
              </div>
              <div class="row">
                <div class="col-lg-6 col-xl-6 col-md-6 col-sm-6 col-12">
                  <div class="social-share-inner-left">
                    <span class="title">find with me</span>
                    <ul class="social-share d-flex liststyle">
                      <li
                        v-for="(elm, i) in socials.slice(0, 3)"
                        :key="i"
                        class=""
                      >
                        <a :href="elm.link"><i :data-feather="elm.icon"></i></a>
                      </li>
                    </ul>
                  </div>
                </div>
                <div
                  class="col-lg-6 col-xl-6 col-md-6 col-sm-6 col-12 mt_mobile--30"
                >
                  <div class="skill-share-inner">
                    <span class="title">best skill on</span>
                    <ul class="skill-share d-flex liststyle">
                      <li v-for="(elm, i) in skillsHero" :key="i">
                        <nuxt-img :src="elm.src" alt="Icons Images" />
                      </li>
                    </ul>
                  </div>
                </div>
              </div>
            </div>
          </div>

          <div class="order-1 order-lg-2 col-lg-5">
            <div class="thumbnail">
              <div class="inner">
                <nuxt-img
                  :width="700"
                  :height="960"
                  src="/assets/images/slider/banner-01.png"
                  alt="Personal Portfolio Images"
                />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import Typed from "typed.js";
import { skillsHero } from "~/data/skills";
import { socials } from "~/data/socials";
const typeitInstance = ref();

onMounted(() => {
  typeitInstance.value = new Typed(".is-visible-one", {
    strings: [" Developer.", " Professional Coder.", " Developer."],
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
