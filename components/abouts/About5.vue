<template>
  <div
    id="about"
    class="d-flex flex-wrap align-content-start h-100 scrollSpysection"
  >
    <div
      class="sticky-top-slider position-sticky sticky-top rbt-sticky-top-adjust-two"
    >
      <div class="banner-details-wrapper-sticky slide">
        <div class="thumbnail">
          <nuxt-img
            :width="500"
            :height="500"
            src="/assets/images/slider/banner-06.png"
            alt="Personal Portfolio"
          />
        </div>
        <div class="banner-title-area pt--30">
          <h1 class="title">
            Hi, I’m <span>Jone Lee</span><br /><span class="span">
              Software Engineer.</span
            >
          </h1>
          <p class="disc">
            I'm the Front-End Developer for #Company in Bangladesh, OR. I have
            serious passion for UI effects, animations and creating intuitive,
            dynamic user experiences.
          </p>
        </div>
        <div
          class="button-group text-center text-md-start pt--60 pt_md--40 pt_sm--40"
        >
          <a class="rn-btn" href="/cv.pdf" download
            ><span>Download My CV</span></a
          >
          <a class="rn-btn" href="#contacts"><span>Hire Me</span></a>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped></style>
