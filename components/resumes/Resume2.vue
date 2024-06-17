<template>
  <div class="container scrollSpysection" id="resume">
    <!-- resume area start -->
    <div class="personal-experience-inner">
      <div class="row">
        <div class="personal-experience-inner">
          <div class="row m--0">
            <!-- Start Skill List Area  -->
            <div class="col-lg-6 col-md-12 col-12">
              <div class="content">
                <span class="subtitle">2007 - 2010</span>
                <h4 class="maintitle">Education Quality</h4>
                <div class="experience-list padding-none border-none">
                  <!-- Start Single List  -->
                  <div class="resume-single-list mt--30">
                    <div class="inner psudo-after-none psudo-after-none">
                      <div class="heading">
                        <div class="title">
                          <h4>Personal Portfolio April Fools</h4>
                          <span>University of DVI (1997 - 2001)</span>
                        </div>
                        <div class="date-of-time">
                          <span>4.30/5</span>
                        </div>
                      </div>
                      <p class="description">
                        The education should be very interactual. Ut tincidunt
                        est ac dolor aliquam sodales. Phasellus sed mauris
                        hendrerit, laoreet sem in, lobortis mauris hendrerit
                        ante.
                      </p>
                    </div>
                  </div>
                  <!-- End Single List  -->

                  <!-- Start Single List  -->
                  <div class="resume-single-list mt--30">
                    <div class="inner psudo-after-none">
                      <div class="heading">
                        <div class="title">
                          <h4>Examples Of Personal Portfolio</h4>
                          <span>College of Studies (2000 - 2002)</span>
                        </div>
                        <div class="date-of-time">
                          <span>4.50/5</span>
                        </div>
                      </div>
                      <p class="description">
                        Maecenas finibus nec sem ut imperdiet. Ut tincidunt est
                        ac dolor aliquam sodales. Phasellus sed mauris
                        hendrerit, laoreet sem in, lobortis mauris hendrerit
                        ante.
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
                <div class="experience-list padding-none border-none">
                  <!-- Start Single List  -->
                  <div class="resume-single-list mt--30">
                    <div class="inner psudo-after-none">
                      <div class="heading">
                        <div class="title">
                          <h4>Diploma in Web Development</h4>
                          <span>BSE In CSE (2004 - 2008)</span>
                        </div>
                        <div class="date-of-time">
                          <span>4.70/5</span>
                        </div>
                      </div>
                      <p class="description">
                        Contrary to popular belief. Ut tincidunt est ac dolor
                        aliquam sodales. Phasellus sed mauris hendrerit, laoreet
                        sem in, lobortis mauris hendrerit ante.
                      </p>
                    </div>
                  </div>
                  <!-- End Single List  -->

                  <!-- Start Single List  -->
                  <div class="resume-single-list mt--30">
                    <div class="inner psudo-after-none">
                      <div class="heading">
                        <div class="title">
                          <h4>The Personal Portfolio Mystery</h4>
                          <span>Job at Rainbow-Themes (2008 - 2016)</span>
                        </div>
                        <div class="date-of-time">
                          <span>4.95/5</span>
                        </div>
                      </div>
                      <p class="description">
                        Generate Lorem Ipsum which looks. Ut tincidunt est ac
                        dolor aliquam sodales. Phasellus sed mauris hendrerit,
                        laoreet sem in, lobortis mauris hendrerit ante.
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
    </div>
    <!-- resume area End -->
    <div class="row mt--50">
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
                <CommonLineProgressbar :percentage="elm.percentage" />
              </div>
            </div>
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
                <CommonLineProgressbar :percentage="elm.percentage" />
              </div>
            </div>
            <!-- End Single Progress Charts -->
          </div>
        </div>
      </div>
      <!-- End Single Progressbar  -->
    </div>
  </div>
</template>

<script setup>
import { skillsetData4, skillsetData5 } from "~/data/skills";
</script>

<style lang="scss" scoped></style>
