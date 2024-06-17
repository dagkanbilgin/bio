<template>
  <div id="about" class="rn-about-area rn-section-gap scrollSpysection">
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
                :width="900"
                :height="1200"
                :src="
                  !isWhiteMode
                    ? '/assets/images/about/about-6.jpg'
                    : '/assets/images/about/about-doctor-white.jpg'
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
              <span class="subtitle">ABOUT ME</span>
              <h2 class="title">Dr. Laura Jerry</h2>
            </div>
            <p class="discription body-color">
              Dr. Laura Jerry brings a wealth of experience and expertise to her
              practice. With a focus on patient-centered care, she is known for
              her warm and empathetic approach, always taking the time to listen
              to her patients’ concerns. Her extensive medical knowledge and
              dedication to staying at the forefront of the field make her a
              trusted healthcare partner.
            </p>
            <p class="discription body-color">
              Explore the range of medical services Dr. Collins offers,
              including general check-ups, preventative care, chronic disease
              management, and more. She is committed to working with you to
              develop personalized treatment plans that suit your unique needs.
            </p>
            <a class="rn-btn" href="#contacts"><span>Learn more</span></a>
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
