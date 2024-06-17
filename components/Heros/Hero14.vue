<template>
  <div id="home" class="rn-slider-area scrollSpysection">
    <div class="slide slider-style-1" style="padding-top: 120px">
      <div class="container">
        <div class="row row--30 align-items-center">
          <div
            class="order-1 order-lg-1 col-lg-6 mt_md--50 mt_sm--50 mt_lg--30"
          >
            <div class="content">
              <div class="inner" style="margin-bottom: 0px">
                <span class="subtitle">HI THERE! I'M</span>
                <h1 class="title">
                  A Senior UX Designer <span>Jone Lee</span>
                  <div class="title2">based in New York, USA</div>
                </h1>

                <div>
                  <p class="description">
                    Designing intuitive, I use animation as a third dimension by
                    which to simplify experiences.
                  </p>
                  <a class="rn-btn" target="_blank" href="#about"
                    ><span>About Me</span></a
                  >
                </div>
              </div>
            </div>
          </div>

          <div class="order-2 order-lg-2 col-lg-6">
            <div class="thumbnail2">
              <div class="inner">
                <nuxt-img
                  :width="640"
                  :height="610"
                  src="/assets/images/slider/banner11.png"
                  alt="Personal Portfolio Images"
                />
              </div>
            </div>
          </div>
        </div>
        <ClientsClients4 />
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped></style>
