<template>
  <div id="home" class="rn-slider-area scrollSpysection">
    <div class="slide slider-style-1 with-square-box">
      <div class="container">
        <div class="row row--30 align-items-center">
          <div
            class="order-2 order-lg-1 col-lg-7 mt_md--50 mt_sm--50 mt_lg--30"
          >
            <div class="content">
              <div class="inner">
                <span class="subtitle">Welcome to my world</span>
                <h1 class="title">
                  Hi, I’m <span>Jone Lee</span><br /><span class="span">
                    UI/UX Designer.</span
                  >
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

          <div class="order-1 order-lg-2 col-lg-5 position-relative">
            <a
              @click="videoPopupActive = true"
              id="play-video"
              class="video-play-button cursor-pointer"
            >
              <span></span>
            </a>
            <div class="thumbnail style-2">
              <div class="inner">
                <nuxt-img
                  :width="520"
                  :height="597"
                  class="w-100"
                  src="/assets/images/slider/banner-03.png"
                  alt="Personal Portfolio Images"
                />
              </div>
            </div>
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
import { skillsHero } from "~/data/skills";
import { socials } from "~/data/socials";
const videoPopupActive = ref(false);
</script>

<style lang="scss" scoped></style>
