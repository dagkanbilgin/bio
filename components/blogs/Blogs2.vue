<template>
  <div class="rn-blog-area scrollSpysection" id="blog">
    <div class="container">
      <div class="row mt-dec-30">
        <!-- Start Single blog -->
        <div
          v-for="(elm, i) in blogs"
          :key="i"
          data-aos="fade-up"
          data-aos-duration="500"
          data-aos-delay="400"
          data-aos-once="true"
          class="col-lg-6 col-xl-4 mt--30 col-md-6 col-sm-12 col-12 mt--30"
        >
          <div
            class="rn-blog"
            data-bs-toggle="modal"
            @click="currentBlogModal = elm"
            data-bs-target="#exampleModalCenters"
          >
            <div class="inner">
              <div class="thumbnail">
                <a href="javascript:void(0)">
                  <nuxt-img :src="elm.imgSrc" alt="Personal Portfolio Images" />
                </a>
              </div>
              <div class="content">
                <div class="category-info">
                  <div class="category-list">
                    <a href="javascript:void(0)">{{ elm.category }}</a>
                  </div>
                  <div class="meta">
                    <span
                      ><i class="feather-clock"></i> {{ elm.readTime }}</span
                    >
                  </div>
                </div>
                <h4 class="title">
                  <a href="javascript:void(0)"
                    >{{ elm.title }} <i class="feather-arrow-up-right"></i
                  ></a>
                </h4>
              </div>
            </div>
          </div>
        </div>
        <!-- End Single blog -->

        <!-- End Single blog -->
      </div>
      <div class="row mt--40">
        <div class="col-12 text-center">
          <a class="rn-btn" href="#">See More <i class="feather-loader"></i></a>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { currentBlogModal } from "~/context/modalContent";
import { blogs } from "~/data/blogs";
</script>

<style lang="scss" scoped></style>
