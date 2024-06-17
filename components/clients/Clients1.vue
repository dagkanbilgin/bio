<template>
  <div
    class="rn-client-area rn-section-gap section-separator scrollSpysection"
    id="clients"
  >
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <div class="section-title">
            <span class="subtitle">Popular Clients</span>
            <h2 class="title">Awesome Clients</h2>
          </div>
        </div>
      </div>

      <div class="row row--25 mt--50 mt_md--40 mt_sm--40">
        <div class="col-lg-4">
          <div class="d-flex flex-wrap align-content-start h-100">
            <div
              class="position-sticky clients-wrapper sticky-top rbt-sticky-top-adjust"
            >
              <ul
                class="nav tab-navigation-button flex-column nav-pills me-3"
                id="v-pills-tab"
                role="tablist"
              >
                <li class="nav-item">
                  <a
                    class="nav-link active"
                    id="v-pills-all-tabs"
                    data-bs-toggle="tab"
                    href="#v-pills-all"
                    role="tab"
                    aria-selected="true"
                    >All</a
                  >
                </li>
                <li class="nav-item">
                  <a
                    class="nav-link"
                    id="v-pills-home-tab"
                    data-bs-toggle="tab"
                    href="#v-pills-Javascript"
                    role="tab"
                    aria-selected="true"
                    >JavaScript</a
                  >
                </li>

                <li class="nav-item">
                  <a
                    class="nav-link"
                    id="v-pills-profile-tab"
                    data-bs-toggle="tab"
                    href="#v-pills-Design"
                    role="tab"
                    aria-selected="true"
                    >Product Design</a
                  >
                </li>

                <li class="nav-item">
                  <a
                    class="nav-link"
                    id="v-pills-wordpress-tab"
                    data-bs-toggle="tab"
                    href="#v-pills-Wordpress"
                    role="tab"
                    aria-selected="true"
                    >Wordpress</a
                  >
                </li>

                <li class="nav-item">
                  <a
                    class="nav-link"
                    id="v-pills-settings-tabs"
                    data-bs-toggle="tab"
                    href="#v-pills-settings"
                    role="tab"
                    aria-selected="true"
                    >HTML to React</a
                  >
                </li>

                <li class="nav-item">
                  <a
                    class="nav-link"
                    id="v-pills-laravel-tabs"
                    data-bs-toggle="tab"
                    href="#v-pills-laravel"
                    role="tab"
                    aria-selected="true"
                    >React To Laravel</a
                  >
                </li>
              </ul>
            </div>
          </div>
        </div>

        <div class="col-lg-8">
          <div class="tab-area">
            <div class="d-flex align-items-start">
              <div class="tab-content w-100" id="v-pills-tabContent">
                <div
                  class="tab-pane fade show active"
                  id="v-pills-all"
                  role="tabpanel"
                  aria-labelledby="v-pills-all-tabs"
                >
                  <div class="client-card">
                    <!-- Start Single Brand  -->
                    <div
                      v-for="(elm, i) in clients2"
                      :key="i"
                      class="main-content"
                    >
                      <div class="inner text-center">
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

                    <!-- End Single Brand  -->
                  </div>
                </div>

                <div
                  class="tab-pane fade"
                  id="v-pills-Javascript"
                  role="tabpanel"
                  aria-labelledby="v-pills-home-tab"
                >
                  <div class="client-card">
                    <!-- Start Single Brand  -->
                    <div
                      v-for="(elm, i) in clients2.filter(
                        (elm) => elm.category == 'JavaScript'
                      )"
                      :key="i"
                      class="main-content"
                    >
                      <div class="inner text-center">
                        <div class="thumbnail">
                          <a href="#"
                            ><nuxt-img
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

                    <!-- End Single Brand  -->
                  </div>
                </div>

                <div
                  class="tab-pane fade"
                  id="v-pills-Design"
                  role="tabpanel"
                  aria-labelledby="v-pills-profile-tab"
                >
                  <div class="client-card">
                    <!-- Start Single Brand  -->
                    <div
                      v-for="(elm, i) in clients2.filter(
                        (elm) => elm.category == 'Product Design'
                      )"
                      :key="i"
                      class="main-content"
                    >
                      <div class="inner text-center">
                        <div class="thumbnail">
                          <a href="#"
                            ><nuxt-img
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

                    <!-- End Single Brand  -->
                  </div>
                </div>

                <div
                  class="tab-pane fade"
                  id="v-pills-Wordpress"
                  role="tabpanel"
                  aria-labelledby="v-pills-wordpress-tab"
                >
                  <div class="client-card">
                    <!-- Start Single Brand  -->
                    <div
                      v-for="(elm, i) in clients2.filter(
                        (elm) => elm.category == 'Wordpress'
                      )"
                      :key="i"
                      class="main-content"
                    >
                      <div class="inner text-center">
                        <div class="thumbnail">
                          <a href="#"
                            ><nuxt-img
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

                    <!-- End Single Brand  -->
                  </div>
                </div>

                <div
                  class="tab-pane fade"
                  id="v-pills-settings"
                  role="tabpanel"
                  aria-labelledby="v-pills-settings-tabs"
                >
                  <div class="client-card">
                    <!-- Start Single Brand  -->
                    <div
                      v-for="(elm, i) in clients2.filter(
                        (elm) => elm.category == 'HTML to React'
                      )"
                      :key="i"
                      class="main-content"
                    >
                      <div class="inner text-center">
                        <div class="thumbnail">
                          <a href="#"
                            ><nuxt-img
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

                    <!-- End Single Brand  -->
                  </div>
                </div>

                <div
                  class="tab-pane fade"
                  id="v-pills-laravel"
                  role="tabpanel"
                  aria-labelledby="v-pills-laravel-tabs"
                >
                  <div class="client-card">
                    <!-- Start Single Brand  -->
                    <div
                      v-for="(elm, i) in clients2.filter(
                        (elm) => elm.category == 'React To Laravel'
                      )"
                      :key="i"
                      class="main-content"
                    >
                      <div class="inner text-center">
                        <div class="thumbnail">
                          <a href="#"
                            ><nuxt-img
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

                    <!-- End Single Brand  -->
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { clients2 } from "~/data/clients";
defineProps(["isWhiteMode"]);
</script>

<style lang="scss" scoped></style>
