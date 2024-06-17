<template>
  <div class="container rn-section-gap-2 scrollSpysection" id="skill">
    <div class="personal-experience-inner sr-designer-skills pb--0 mt--40">
      <div class="row">
        <div class="col-lg-12">
          <div class="section-title text-center">
            <span class="subtitle"
              >HERE IS A SAMPLE OF PROJECTS I'VE WORKED ON.</span
            >
            <h2 class="title">Selected projects</h2>
          </div>
        </div>
      </div>
      <div class="row rn-section-gap-2 progressLine2">
        <!-- Start Single Progressbar  -->
        <div class="col-lg-4 col-md-6 col-12 skills-column">
          <div class="progress-wrapper box-area-1">
            <div class="content">
              <span class="subtitle">Skillset One</span>
              <h4 class="maintitle">FACILITATION</h4>
              <!-- Start Single Progress Charts -->

              <div
                v-for="(elm, i) in skillsetData1"
                :key="i"
                class="progress-charts"
              >
                <h6 class="heading heading-h6">{{ elm.skill }}</h6>
                <div class="progress">
                  <CommonLineProgressbar :percentage="elm.percentage" />
                </div>
              </div>
              <!-- End Single Progress Charts -->

              <!-- End Single Progress Charts -->
            </div>
          </div>
        </div>
        <!-- End Single Progressbar  -->

        <!-- Start Single Progressbar  -->
        <div class="col-lg-4 col-md-6 col-12 mt_sm--60 skills-column">
          <div class="progress-wrapper box-area-1">
            <div class="content">
              <span class="subtitle">Skillset Two</span>
              <h4 class="maintitle">UX DESIGN</h4>
              <!-- Start Single Progress Charts -->
              <div
                v-for="(elm, i) in skillsetData2"
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
        <div class="col-lg-4 col-md-6 col-12 mt_sm--60 skills-column">
          <div class="progress-wrapper box-area-1">
            <div class="content">
              <span class="subtitle">Skillset Three</span>
              <h4 class="maintitle">UI DESIGN</h4>
              <!-- Start Single Progress Charts -->
              <div
                v-for="(elm, i) in skillsetData3"
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
    <div class="text-center mt--0">
      I consistently aim to employ the right techniques and methods to attain
      the optimal results.
    </div>
  </div>
</template>

<script setup>
import { skillsetData1, skillsetData2, skillsetData3 } from "~/data/skills";
</script>

<style lang="scss" scoped></style>
