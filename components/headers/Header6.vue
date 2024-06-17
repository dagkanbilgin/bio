<template>
  <CommonMobileMenu :navItems="navItems" />
  <header
    class="rn-header header-6 haeder-default black-logo-version header--fixed header--sticky"
  >
    <div
      class="header-wrapper m--0 rn-popup-mobile-menu row align-items-center"
    >
      <!-- Start Header Left -->
      <div class="col-lg-2 col-6">
        <div class="header-left">
          <div class="logo">
            <nuxt-link to="/">
              <nuxt-img
                class="logo-light logo-light-photographer"
                src="/assets/images/logo/logo.png"
                style="object-fit: contain"
                :width="139"
                :height="70"
                alt="logo-image"
              />
              <nuxt-img
                class="logo-dark logo-dark-photographer"
                src="/assets/images/logo/logo-dark.png"
                style="object-fit: contain"
                :width="139"
                :height="70"
                alt="logo-image"
              />
            </nuxt-link>
          </div>
        </div>
      </div>
      <!-- End Header Left -->
      <!-- Start Header Center -->
      <div class="col-lg-10 col-6">
        <div class="header-center">
          <nav id="sideNav" class="mainmenu-nav navbar-example2 onepagenav">
            <!-- Start Mainmanu Nav -->
            <ul class="primary-menu nav nav-pills scrollspyLinks">
              <HeadersNav :navItems="navItems" />
            </ul>
            <!-- End Mainmanu Nav -->
          </nav>
          <!-- Start Header Right  -->
          <div class="header-right">
            <div class="rbt-mini-cart-wrap only-dark">
              <a href="https://rainbowit.net/themes/inbio/cart/"
                ><span class="mini-cart"
                  ><i class="feather-shopping-cart"></i
                  ><span class="rbt-cart-count">0</span></span
                ></a
              >
            </div>
            <a
              class="rn-btn no-shadow btn-theme"
              target="_blank"
              href="https://themeforest.net/checkout/from_item/33188244?license=regular"
              ><span>BUY NOW</span></a
            >
            <i
              id="menuBtn"
              class="feather-menu humberger-menu d-block d-xl-none"
              @click="menuOpen"
            ></i>
            <div class="close-menu d-block">
              <span class="closeTrigger">
                <i data-feather="x"></i>
              </span>
            </div>
          </div>
          <!-- End Header Right  -->
        </div>
      </div>
      <!-- End Header Center -->
    </div>
  </header>
</template>

<script setup>
import { menuOpen } from "~/utlis/menuToggle";

defineProps(["navItems"]);
</script>

<style lang="scss" scoped></style>
