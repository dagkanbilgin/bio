<template>
  <div
    class="rn-contact-area rn-section-gap section-separator scrollSpysection"
    id="contacts"
  >
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <div class="section-title text-center">
            <span class="subtitle">LET'S MEET!</span>
            <h2 class="title">Hire Me 🚣</h2>
          </div>
        </div>
      </div>

      <div class="row mt--50 mt_md--40 mt_sm--40 mt-contact-sm">
        <div data-aos-delay="600" class="col-lg-12 contact-input">
          <div class="contact-form-wrapper">
            <div class="introduce">
              <form
                class="rnt-contact-form rwt-dynamic-form row"
                @submit.prevent=""
              >
                <div class="col-lg-6">
                  <div class="form-group">
                    <label for="contact-name">Your Name</label>
                    <input
                      class="form-control form-control-lg"
                      name="contact-name"
                      id="contact-name"
                      type="text"
                    />
                  </div>
                </div>

                <div class="col-lg-6">
                  <div class="form-group">
                    <label for="contact-phone">Phone Number</label>
                    <input
                      class="form-control"
                      name="contact-phone"
                      id="contact-phone"
                      type="text"
                    />
                  </div>
                </div>

                <div class="col-lg-12">
                  <div class="form-group">
                    <label for="contact-email">Email</label>
                    <input
                      class="form-control form-control-sm"
                      id="contact-email"
                      name="contact-email"
                      type="email"
                    />
                  </div>
                </div>

                <div class="col-lg-12">
                  <div class="form-group">
                    <label for="subject">subject</label>
                    <input
                      class="form-control form-control-sm"
                      id="subject"
                      name="subject"
                      type="text"
                    />
                  </div>
                </div>

                <div class="col-lg-12">
                  <div class="form-group">
                    <label for="contact-message">Your Message</label>
                    <textarea
                      name="contact-message"
                      id="contact-message"
                      cols="10"
                      rows="10"
                    ></textarea>
                  </div>
                </div>

                <div class="col-lg-12">
                  <button
                    name="submit"
                    type="submit"
                    id="submit"
                    class="rn-btn"
                  >
                    <span>SEND MESSAGE</span>
                    <i data-feather="arrow-right"></i>
                  </button>
                </div>
              </form>
            </div>
          </div>
        </div>
      </div>
      <ul class="contact-links">
        <li class="">
          <a href="#">
            <span class="">
              <i aria-hidden="true" class="rbt feather-facebook"></i>
            </span>
            <span class="">facebook</span>
          </a>
        </li>
        <li class="">
          <a href="#">
            <span class="">
              <i aria-hidden="true" class="rbt feather-instagram"></i>
            </span>
            <span class="">instagram</span>
          </a>
        </li>
        <li class="">
          <a href="#">
            <span class="">
              <i aria-hidden="true" class="rbt feather-link-2"></i>
            </span>
            <span class="">example.com</span>
          </a>
        </li>
        <li class="">
          <span class="">
            <i aria-hidden="true" class="rbt feather-map-pin"></i>
          </span>
          <span class=""> RA, 26 North Street. 23th Floor #353</span>
        </li>
      </ul>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped></style>
