<template>
  <div id="about" class="rn-about-area sr-designer-about scrollSpysection">
    <div class="container">
      <div class="row">
        <div class="col-lg-5">
          <div
            data-aos="fade-up"
            data-aos-duration="1000"
            data-aos-delay="100"
            data-aos-once="true"
            class="image-area"
          >
            <div class="thumbnail">
              <nuxt-img
                :width="444"
                :height="658"
                :src="
                  isWhiteMode
                    ? '/assets/images/about/about-8.jpg'
                    : '/assets/images/about/about-7.jpg'
                "
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
              <h3 class="title">
                Inquisitive and passionate about emerging technology.
              </h3>
            </div>
            <p class="discription body-color">
              I’m Tom Latham, a Senior UX Designer with over 14 years of
              hands-on experience in User Experience, Product Analytics, and
              Strategic Thinking.
            </p>
            <p class="discription body-color">
              Currently, I’m dedicated to creating user experiences that harness
              AI to enhance data visualization, predictive modeling, and
              insights for users across various domains at Qlik.
            </p>
            <p class="discription body-color">
              For a more comprehensive understanding of my qualifications and
              career achievements, please visit my LinkedIn profile .
            </p>
            <a class="rn-btn" href="/cv.pdf" download
              ><span>DOWNLOAD RESUME</span></a
            >
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
defineProps(["isWhiteMode"]);
</script>

<style lang="scss" scoped></style>
