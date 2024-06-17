<template>
  <div class="container rn-section-gap">
    <!-- resume area start -->

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
