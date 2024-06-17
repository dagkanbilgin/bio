<template>
  <div id="about" class="rn-about-area scrollSpysection">
    <div class="container">
      <div class="row">
        <div class="col-lg-5">
          <div
            class="image-area shadow-none padding-none"
            data-aos="fade-up"
            data-aos-duration="1000"
            data-aos-delay="100"
            data-aos-once="true"
          >
            <div class="thumbnail">
              <nuxt-img
                :width="500"
                :height="664"
                src="/assets/images/about/about-2.jpg"
                alt="Personal Portfolio Image"
              />
            </div>
          </div>
        </div>
        <div
          data-aos="fade-up"
          data-aos-duration="1000"
          data-aos-delay="100"
          data-aos-once="true"
          class="col-lg-7 mt_sm--30"
        >
          <div class="contant">
            <div class="section-title text-left">
              <span class="subtitle">Visit my portfolio & Hire me</span>
              <h2 class="title small-h2">About Me</h2>
            </div>
            <p class="discription color-body">
              Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eum in
              eos saepe ipsa cupiditate accusantium voluptatibus quidem nam,
              reprehenderit, et necessitatibus adipisci.
            </p>
            <ul class="about-skill-style mb--40">
              <li v-for="(elm, i) in features5" :key="i">
                <i data-feather="check"></i><span>{{ elm.title }} </span>
              </li>
            </ul>
            <a class="rn-btn" href="/cv.pdf" download
              ><span>DOWNLOAD MY CV</span></a
            >
          </div>
        </div>
      </div>
      <!-- what I am doing area -->
      <div class="row mt--50">
        <div class="col-12 text-center">
          <h6 class="title color-lightn mb--30">What I am Doing</h6>
        </div>
        <div class="col-lg-6 mb_sm--30 mb_md--30">
          <div class="service-card-one border-style">
            <div class="inner">
              <i data-feather="edit"></i>
              <h6 class="title color-lightn">Web Design Full stack</h6>
              <p class="describe">
                Lorem ipsum, dolor sit amet consectetur adipisicing elit.
                Inventore dolorum atque dicta distinctio mollitia fuga.
              </p>
            </div>
          </div>
        </div>
        <div class="col-lg-6">
          <div class="service-card-one border-style">
            <div class="inner">
              <i data-feather="cast"></i>
              <h6 class="title color-lightn">Web Design</h6>
              <p class="describe">
                Lorem ipsum, dolor sit amet consectetur adipisicing elit.
                Inventore dolorum atque dicta distinctio mollitia fuga.
              </p>
            </div>
          </div>
        </div>
      </div>
      <!-- what I am doing area End -->
      <div class="row mt--50">
        <!-- Brand style three -->
        <div class="rn-brand-area">
          <div class="container">
            <div class="row mb--30">
              <div class="col-12 text-center">
                <h6 class="title color-lightn m--0">Our trusted Clients</h6>
              </div>
            </div>
            <div class="row">
              <div class="brand-wrapper-three mb_dec--30">
                <!-- Start Single Brand  -->
                <div
                  v-for="(elm, i) in clients.slice(0, 4)"
                  :key="i"
                  data-aos="fade-up"
                  data-aos-duration="1000"
                  data-aos-delay="300"
                  data-aos-once="true"
                  class="rn-brand flex-basis-style-1"
                >
                  <div
                    class="border-style shadow-none inner smlg-brand text-center"
                  >
                    <div class="thumbnail">
                      <a href="#"
                        ><img
                          :src="isWhiteMode ? elm.imageDark : elm.image"
                          alt="Client-image"
                      /></a>
                    </div>
                    <div class="seperator"></div>
                    <div class="client-name">
                      <span
                        ><a href="#">{{ elm.name }}</a></span
                      >
                    </div>
                  </div>
                </div>

                <!-- End Single Brand  -->
              </div>
            </div>
          </div>
        </div>
        <!-- Brand style three End -->
      </div>
    </div>
  </div>
</template>

<script setup>
defineProps(["isWhiteMode"]);
import { clients } from "~/data/clients";
import { features5 } from "~/data/features";
</script>

<style lang="scss" scoped></style>
