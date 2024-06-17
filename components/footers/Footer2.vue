<template>
  <div
    id="footer"
    class="rn-footer-area footer-style-2 rn-section-gapTop section-separator scrollSpysection"
  >
    <div class="container pb--80 pb_sm--40 plr_sm--20">
      <div class="row">
        <div class="col-xl-3 col-12 col-lg-3 col-md-6 col-sm-6 col-12">
          <div class="logo-thumbnail">
            <nuxt-link to="/">
              <nuxt-img
                :width="139"
                :height="70"
                class="logo-light"
                src="/assets/images/logo/logo.png"
                style="object-fit: contain"
                alt="logo-image"
              />
              <nuxt-img
                :width="139"
                :height="70"
                class="logo-dark"
                src="/assets/images/logo/logo-dark.png"
                style="object-fit: contain"
                alt="logo-image"
              />
            </nuxt-link>
          </div>
          <div class="social-icone-wrapper">
            <ul class="social-share d-flex liststyle">
              <li class="facebook">
                <a href="#"><i data-feather="linkedin"></i></a>
              </li>
              <li class="instagram">
                <a href="#"><i data-feather="instagram"></i></a>
              </li>
              <li class="linkedin">
                <a href="#"><i data-feather="twitter"></i></a>
              </li>
            </ul>
          </div>
        </div>
        <div
          v-for="(menu, index) in footerLinks"
          :key="index"
          class="col-sl-3 col-12 mt_sm--20 col-lg-3 col-md-6 col-sm-6 col-12"
        >
          <div class="menu-wrapper">
            <div class="menu-title">
              <h6>{{ menu.title }}</h6>
            </div>
            <ul class="menu-footer">
              <li v-for="(item, itemIndex) in menu.items" :key="itemIndex">
                <a :href="item.link">{{ item.name }}</a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="copyright text-center ptb--40 section-separator">
      <p class="description">
        © {{ new Date().getFullYear() }}. All rights reserved by
        <a
          target="_blank"
          href="https://themeforest.net/user/rainbow-themes/portfolio"
          >Rainbow-Themes.</a
        >
      </p>
    </div>
  </div>
</template>

<script setup>
import { footerLinks } from "~/data/menu";
</script>

<style lang="scss" scoped></style>
