<template>
  <div id="home" class="rn-slider-area scrollSpysection">
    <!-- Start Single Slide -->
    <div class="slide slider-style-4 bg_image bg_image--1">
      <div class="container">
        <div class="row">
          <div class="order-2 order-lg-1 col-lg-9 col-xl-7">
            <div class="content">
              <div class="inner mb_sm--80">
                <h1 class="title">
                  Hi, I’m <span>Zarin Nes</span><br />
                  <span class="span">Photographer</span>
                </h1>
                <div>
                  <p class="description">
                    I design and code beautifully simple things, and I love what
                    I do. I use animation as a third dimension by which Lorem
                    ipsum dolor sit amet consectetur adipisicing.
                  </p>
                </div>
              </div>
              <div class="row">
                <div class="col-lg-12 col-xl-6 col-md-12 col-sm-12 col-12">
                  <div class="social-share-inner-left">
                    <span class="title">find with me</span>
                    <ul class="social-share d-flex liststyle">
                      <li v-for="(elm, i) in socials" :key="i" class="">
                        <a :href="elm.link"><i :data-feather="elm.icon"></i></a>
                      </li>
                    </ul>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- End Single Slide -->
  </div>
</template>

<script setup>
import { socials } from "~/data/socials";
</script>

<style lang="scss" scoped></style>
