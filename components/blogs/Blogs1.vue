<template>
  <div
    class="rn-blog-area rn-section-gap section-separator scrollSpysection mw-100"
    id="blog"
  >
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <div
            data-aos="fade-up"
            data-aos-duration="500"
            data-aos-delay="100"
            data-aos-once="true"
            class="section-title text-center"
          >
            <span class="subtitle">Visit my blog and keep your feedback</span>
            <h2 class="title">My Blog</h2>
          </div>
        </div>
      </div>
      <div class="row row--25 mt--30 mt_md--10 mt_sm--10">
        <!-- Start Single blog -->
        <div
          v-for="(elm, i) in blogs.slice(0, 3)"
          :key="i"
          data-aos="fade-up"
          data-aos-duration="500"
          data-aos-delay="100"
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
      </div>
    </div>
  </div>
</template>

<script setup>
import { currentBlogModal } from "~/context/modalContent";
import { blogs } from "~/data/blogs";
</script>

<style lang="scss" scoped></style>
