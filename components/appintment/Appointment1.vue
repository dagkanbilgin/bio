<template>
  <div
    class="rn-resume-area rn-section-gap section-separator scrollSpysection"
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
                >RC Medical College</a
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
                >Delta Hospital</a
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
                >United Hospital</a
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
              >
                Squre Hospital</a
              >
            </li>
          </ul>

          <!-- Start Tab Content Wrapper  -->
          <div class="rn-nav-content tab-content" id="myTabContents">
            <!-- Start Single Tab  -->
            <div
              v-for="(tab, index) in appintmentTabs"
              :key="index"
              :class="['tab-pane', { 'show active fade': index === 0 }]"
              :id="tab.id"
              role="tabpanel"
              :aria-labelledby="tab.ariaLabelledBy"
            >
              <div
                style="
                  width: 100%;
                  margin-top: 40px;
                  padding: 0;
                  overflow: hidden;
                "
                class="contact-about-area appintment-card"
              >
                <div class="row" :class="{ 'row-reverse': tab.reverseOrder }">
                  <div
                    class="col-lg-7 appintment-content"
                    :class="{ 'order-2': tab.reverseOrder }"
                  >
                    <div class="title-area">
                      <span>{{ tab.title }}</span>
                      <h4 class="title mt-5">{{ tab.subtitle }}</h4>
                    </div>
                    <ul class="addresslist">
                      <li
                        class="addressitem"
                        v-for="(item, i) in tab.addressItems"
                        :key="i"
                      >
                        <strong class=""
                          ><i class="feather" :class="item.iconClass"></i
                        ></strong>
                        <span class="list-content"
                          >{{ item.content.label }}:
                          <strong>{{ item.content.value }}</strong>
                        </span>
                      </li>
                    </ul>
                    <div class="section-separator mt-5"></div>
                    <div
                      class="mt-5"
                      style="font-size: 16px; padding-top: 40px"
                    >
                      Call For Appointment {{ tab.appointmentNumber }}
                    </div>
                  </div>
                  <div
                    class="col-lg-5"
                    :class="{ 'order-1': tab.reverseOrder }"
                  >
                    <nuxt-img
                      style="height: 100%; object-fit: cover"
                      :src="tab.imageSrc"
                      alt="image"
                    />
                  </div>
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
import { appintmentTabs } from "~/data/appintments";
</script>

<style lang="scss" scoped></style>
