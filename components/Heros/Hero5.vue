<template>
  <div id="home" class="rn-slide-area scrollSpysection">
    <div class="slide slider-style-3">
      <div class="container">
        <div class="row slider-wrapper">
          <div
            class="order-2 order-xl-1 col-lg-12 col-xl-5 mt_lg--50 mt_md--50 mt_sm--50"
          >
            <div class="slider-info">
              <div class="row">
                <div class="col-xl-12 col-lg-12 col-12">
                  <div class="user-info-top">
                    <div class="user-info-header">
                      <div class="user">
                        <i data-feather="user"></i>
                      </div>
                      <h2 class="title">Hi, I’m <span>InBio</span></h2>
                      <p class="disc">
                        Web designer and developer working for envato.com in
                        Paris, France.
                      </p>
                    </div>
                    <div class="user-info-footer">
                      <div class="info">
                        <i data-feather="file"></i>
                        <span>Web designer & developer</span>
                      </div>
                      <div class="info">
                        <i data-feather="mail"></i>
                        <span>john.slady@gmail.com</span>
                      </div>
                      <div class="info">
                        <i data-feather="map-pin"></i>
                        <span>Paris fan</span>
                      </div>
                    </div>
                  </div>
                </div>

                <div class="col-xl-12 col-lg-12 col-12">
                  <div class="user-info-bottom">
                    <span>Download my curriculum vitae: </span>
                    <div class="button-wrapper d-flex">
                      <a class="rn-btn mr--30" href="/cv.pdf" download
                        ><span>DOWNLOAD CV</span></a
                      >
                      <a class="rn-btn" href="#contacts"
                        ><span>CONTACT ME</span></a
                      >
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>

          <div class="order-1 order-xl-2 col-lg-12 col-xl-7">
            <div class="background-image-area">
              <div class="thumbnail-image">
                <nuxt-img
                  :width="800"
                  :height="600"
                  src="/assets/images/slider/banner-02.png"
                  alt="Personal Portfolio"
                />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped></style>
