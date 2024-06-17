<template>
  <div
    class="rn-resume-area rn-section-gap section-separator scrollSpysection mw-100"
    id="resume"
  >
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <div class="section-title text-center">
            <span class="subtitle">7+ Years of Experience</span>
            <h2 class="title">My Resume</h2>
          </div>
        </div>
      </div>
      <div class="row mt--45">
        <div class="col-lg-12">
          <ul class="rn-nav-list nav nav-tabs" id="myTabs" role="tablist">
            <li class="nav-item">
              <a
                class="nav-link active"
                id="education-tab"
                data-bs-toggle="tab"
                href="#education"
                role="tab"
                aria-controls="education"
                aria-selected="true"
                >education</a
              >
            </li>
            <li class="nav-item">
              <a
                class="nav-link"
                id="professional-tab"
                data-bs-toggle="tab"
                href="#professional"
                role="tab"
                aria-controls="professional"
                aria-selected="false"
                >professional Skills</a
              >
            </li>
            <li class="nav-item">
              <a
                class="nav-link"
                id="experience-tab"
                data-bs-toggle="tab"
                href="#experience"
                role="tab"
                aria-controls="experience"
                aria-selected="false"
                >experience</a
              >
            </li>
            <li class="nav-item">
              <a
                class="nav-link"
                id="interview-tab"
                data-bs-toggle="tab"
                href="#interview"
                role="tab"
                aria-controls="interview"
                aria-selected="false"
                >interview</a
              >
            </li>
          </ul>

          <!-- Start Tab Content Wrapper  -->
          <div class="rn-nav-content tab-content" id="myTabContents">
            <!-- Start Single Tab  -->
            <div
              class="tab-pane show active fade single-tab-area"
              id="education"
              role="tabpanel"
              aria-labelledby="education-tab"
            >
              <div class="personal-experience-inner mt--40">
                <div class="row">
                  <!-- Start Skill List Area  -->
                  <div class="col-lg-6 col-md-12 col-12">
                    <div class="content">
                      <span class="subtitle">2007 - 2010</span>
                      <h4 class="maintitle">Education Quality</h4>
                      <div class="experience-list">
                        <!-- Start Single List  -->
                        <div
                          v-for="(elm, i) in education2"
                          :key="i"
                          class="resume-single-list"
                        >
                          <div class="inner">
                            <div class="heading">
                              <div class="title">
                                <h4>{{ elm.title }}</h4>
                                <span>{{ elm.institution }}</span>
                              </div>
                              <div class="date-of-time">
                                <span>{{ elm.rating }}</span>
                              </div>
                            </div>
                            <p class="description">
                              {{ elm.description }}
                            </p>
                          </div>
                        </div>
                        <!-- End Single List  -->

                        <!-- End Single List  -->
                      </div>
                    </div>
                  </div>
                  <!-- End Skill List Area  -->

                  <!-- Start Skill List Area 2nd  -->
                  <div class="col-lg-6 col-md-12 col-12 mt_md--60 mt_sm--60">
                    <div class="content">
                      <span class="subtitle">2007 - 2010</span>
                      <h4 class="maintitle">Job Experience</h4>
                      <div class="experience-list">
                        <!-- Start Single List  -->
                        <div
                          v-for="(elm, i) in education3"
                          :key="i"
                          class="resume-single-list"
                        >
                          <div class="inner">
                            <div class="heading">
                              <div class="title">
                                <h4>{{ elm.title }}</h4>
                                <span>{{ elm.institution }}</span>
                              </div>
                              <div class="date-of-time">
                                <span>{{ elm.rating }}</span>
                              </div>
                            </div>
                            <p class="description">
                              {{ elm.description }}
                            </p>
                          </div>
                        </div>
                        <!-- End Single List  -->
                      </div>
                    </div>
                  </div>
                  <!-- End Skill List Area  -->
                </div>
              </div>
            </div>
            <!-- End Single Tab  -->

            <!-- Start Single Tab  -->
            <div
              class="tab-pane fade"
              id="professional"
              role="tabpanel"
              aria-labelledby="professional-tab"
            >
              <div class="personal-experience-inner mt--40">
                <div class="row row--40">
                  <!-- Start Single Progressbar  -->
                  <div class="col-lg-6 col-md-6 col-12">
                    <div class="progress-wrapper">
                      <div class="content">
                        <span class="subtitle">Features</span>
                        <h4 class="maintitle">Design Skill</h4>
                        <!-- Start Single Progress Charts -->
                        <div
                          v-for="(elm, i) in skillsetData4"
                          :key="i"
                          class="progress-charts"
                        >
                          <h6 class="heading heading-h6">{{ elm.skill }}</h6>
                          <div class="progress">
                            <CommonLineProgressbar
                              :percentage="elm.percentage"
                            />
                          </div>
                        </div>
                        <!-- End Single Progress Charts -->

                        <!-- End Single Progress Charts -->
                      </div>
                    </div>
                  </div>
                  <!-- End Single Progressbar  -->

                  <!-- Start Single Progressbar  -->
                  <div class="col-lg-6 col-md-6 col-12 mt_sm--60">
                    <div class="progress-wrapper">
                      <div class="content">
                        <span class="subtitle">Features</span>
                        <h4 class="maintitle">Development Skill</h4>
                        <!-- Start Single Progress Charts -->
                        <div
                          v-for="(elm, i) in skillsetData5"
                          :key="i"
                          class="progress-charts"
                        >
                          <h6 class="heading heading-h6">{{ elm.skill }}</h6>
                          <div class="progress">
                            <CommonLineProgressbar
                              :percentage="elm.percentage"
                            />
                          </div>
                        </div>
                        <!-- End Single Progress Charts -->
                      </div>
                    </div>
                  </div>
                  <!-- End Single Progressbar  -->
                </div>
              </div>
            </div>
            <!-- End Single Tab  -->

            <!-- Start Single Tab  -->
            <div
              class="tab-pane fade"
              id="experience"
              role="tabpanel"
              aria-labelledby="experience-tab"
            >
              <div class="personal-experience-inner mt--40">
                <div class="row">
                  <!-- Start Skill List Area  -->
                  <div class="col-lg-6 col-md-12 col-12">
                    <div class="content">
                      <span class="subtitle">2007 - 2010</span>
                      <h4 class="maintitle">Education Quality</h4>
                      <div class="experience-list">
                        <div
                          v-for="(elm, i) in education2"
                          :key="i"
                          class="resume-single-list"
                        >
                          <div class="inner">
                            <div class="heading">
                              <div class="title">
                                <h4>{{ elm.title }}</h4>
                                <span>{{ elm.institution }}</span>
                              </div>
                              <div class="date-of-time">
                                <span>{{ elm.rating }}</span>
                              </div>
                            </div>
                            <p class="description">
                              {{ elm.description }}
                            </p>
                          </div>
                        </div>
                      </div>
                    </div>
                  </div>
                  <!-- End Skill List Area  -->

                  <!-- Start Skill List Area 2nd  -->
                  <div class="col-lg-6 col-md-12 col-12 mt_md--60 mt_sm--60">
                    <div class="content">
                      <span class="subtitle">2007 - 2010</span>
                      <h4 class="maintitle">Job Experience</h4>
                      <div class="experience-list">
                        <!-- Start Single List  -->
                        <div
                          v-for="(elm, i) in education3"
                          :key="i"
                          class="resume-single-list"
                        >
                          <div class="inner">
                            <div class="heading">
                              <div class="title">
                                <h4>{{ elm.title }}</h4>
                                <span>{{ elm.institution }}</span>
                              </div>
                              <div class="date-of-time">
                                <span>{{ elm.rating }}</span>
                              </div>
                            </div>
                            <p class="description">
                              {{ elm.description }}
                            </p>
                          </div>
                        </div>

                        <!-- End Single List  -->
                      </div>
                    </div>
                  </div>
                  <!-- End Skill List Area  -->
                </div>
              </div>
            </div>
            <!-- End Single Tab  -->

            <!-- Start Single Tab  -->
            <div
              class="tab-pane fade"
              id="interview"
              role="tabpanel"
              aria-labelledby="interview-tab"
            >
              <div class="personal-experience-inner mt--40">
                <div class="row">
                  <!-- Start Skill List Area  -->
                  <div class="col-lg-6 col-md-12 col-12">
                    <div class="content">
                      <span class="subtitle">2007 - 2010</span>
                      <h4 class="maintitle">Company Experience</h4>
                      <div class="experience-list">
                        <!-- Start Single List  -->
                        <div
                          v-for="(elm, i) in education2"
                          :key="i"
                          class="resume-single-list"
                        >
                          <div class="inner">
                            <div class="heading">
                              <div class="title">
                                <h4>{{ elm.title }}</h4>
                                <span>{{ elm.institution }}</span>
                              </div>
                              <div class="date-of-time">
                                <span>{{ elm.rating }}</span>
                              </div>
                            </div>
                            <p class="description">
                              {{ elm.description }}
                            </p>
                          </div>
                        </div>
                        <!-- End Single List  -->
                      </div>
                    </div>
                  </div>
                  <!-- End Skill List Area  -->

                  <!-- Start Skill List Area 2nd  -->
                  <div class="col-lg-6 col-md-12 col-12 mt_md--60 mt_sm--60">
                    <div class="content">
                      <span class="subtitle">2007 - 2010</span>
                      <h4 class="maintitle">Job Experience</h4>
                      <div class="experience-list">
                        <div
                          v-for="(elm, i) in education3"
                          :key="i"
                          class="resume-single-list"
                        >
                          <div class="inner">
                            <div class="heading">
                              <div class="title">
                                <h4>{{ elm.title }}</h4>
                                <span>{{ elm.institution }}</span>
                              </div>
                              <div class="date-of-time">
                                <span>{{ elm.rating }}</span>
                              </div>
                            </div>
                            <p class="description">
                              {{ elm.description }}
                            </p>
                          </div>
                        </div>
                        <!-- End Single List  -->
                      </div>
                    </div>
                  </div>
                  <!-- End Skill List Area  -->
                </div>
              </div>
            </div>
            <!-- End Single Tab  -->
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { education2, education3 } from "~/data/education";
import { skillsetData4, skillsetData5 } from "~/data/skills";
</script>

<style lang="scss" scoped></style>
