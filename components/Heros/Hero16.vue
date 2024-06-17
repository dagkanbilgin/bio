<template>
  <div id="home" class="rn-slider-area scrollSpysection">
    <div class="slide slider-style-1 lawer-hero-section">
      <div class="container">
        <div class="row row--40 align-items-center">
          <div class="col-lg-4 col-md-12">
            <div class="thumbnail box-gradient-2">
              <div class="inner w-100">
                <nuxt-img
                  v-if="isWhiteMode"
                  style="height: 100%; object-fit: cover"
                  class="w-100"
                  src="/assets/images/lawers/lawyer-laight-banner.png"
                  alt="Personal Portfolio Images"
                />
                <nuxt-img
                  v-else
                  :width="512"
                  :height="555"
                  style="height: 100%; object-fit: cover"
                  class="w-100"
                  src="/assets/images/slider/lawyer-single-profile.jpg"
                  alt="Personal Portfolio Images"
                />
              </div>
            </div>
            <div class="experience mt-4">
              <span class="experience-year"> 27+ </span>
              <span> Years experiences </span>
            </div>
          </div>
          <div class="col-lg-4 col-md-12 mt_md--50 mt_sm--50">
            <div class="content">
              <div class="inner" style="margin-bottom: 0px !important">
                <span class="subtitle">ATTORNEY</span>
                <h3 class="title title2" style="line-height: 1.1">
                  Hi, I’m Advocate <span>Jone Lee</span><br /><span
                    class="place"
                  >
                    based in <span class="place is-visible-one"></span
                  ></span>
                </h3>
                <div>
                  <p class="description">
                    California-based lawyers aim to consistently enhance
                  </p>
                </div>
                <div class="section-separator mt-5 pb-5"></div>
                <div class="social-share-inner-left">
                  <span class="text">find with me</span>
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
            </div>
          </div>

          <div
            data-aos-delay="600"
            class="col-lg-4 col-md-12 contact-input lawer-hero-contact mt-sm-5"
          >
            <div class="contact-form-wrapper ml-0">
              <div class="introduce">
                <form
                  class="rnt-contact-form rwt-dynamic-form row"
                  @submit.prevent=""
                >
                  <div class="col-lg-12">
                    <div class="form-group">
                      <label for="contact-email">Email</label>
                      <input
                        class="form-control form-control-sm"
                        id="contact-email"
                        name="contact-email"
                        type="email"
                      />
                    </div>
                  </div>

                  <div class="col-lg-12">
                    <div class="form-group">
                      <label for="contact-message">Your Message</label>
                      <textarea
                        class="hero-text-area"
                        name="contact-message"
                        id="contact-message"
                        cols="30"
                        rows="5"
                      ></textarea>
                    </div>
                  </div>

                  <div class="col-lg-12">
                    <button
                      name="submit"
                      type="submit"
                      id="submit"
                      class="rn-btn"
                    >
                      <span>SEND MESSAGE</span>
                      <i data-feather="arrow-right"></i>
                    </button>
                  </div>
                </form>
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
import { socials } from "~/data/socials";
const typeitInstance = ref();
defineProps(["isWhiteMode"]);
onMounted(() => {
  typeitInstance.value = new Typed(".is-visible-one", {
    strings: [" USA.", " UK.", " UAE."],
    typeSpeed: 86,
    backSpeed: 80,
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
