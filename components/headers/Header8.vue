<template>
  <CommonMobileMenu2 />
  <header
    class="rn-header haeder-default inbio-default-header overflow-visible"
  >
    <div
      class="header-wrapper rn-popup-mobile-menu m--0 row align-items-center"
    >
      <!-- Start Header Left -->
      <div class="col-lg-2 col-6">
        <div class="header-left">
          <div class="logo">
            <nuxt-link to="/">
              <nuxt-img
                class="logo-light"
                src="/assets/images/logo/logo.png"
                style="object-fit: contain"
                :width="139"
                :height="70"
                alt="logo-image"
              />
              <nuxt-img
                class="logo-dark"
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
          <nav class="mainmenu-nav d-none d-xl-block">
            <ul class="primary-menu">
              <li class="nav-item"><a class="nav-link" href="#">Home</a></li>
              <li class="nav-item">
                <a class="nav-link" href="#">Experience</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#">Education</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#">Resume</a>
              </li>
              <li class="nav-item has-droupdown">
                <a class="nav-link" href="#">Pages</a>
                <ul class="submenu">
                  <li v-for="(elm, i) in menuItemsElementPages" :key="i">
                    <nuxt-link :to="elm.href">{{ elm.title }}</nuxt-link>
                  </li>
                </ul>
              </li>
              <li class="nav-item"><a class="nav-link" href="#">Blog</a></li>
              <li class="nav-item">
                <a class="nav-link" href="#">Footer</a>
              </li>
            </ul>
          </nav>
          <!-- Start Header Right  -->
          <div class="header-right">
            <div class="rbt-mini-cart-wrap">
              <a href="https://rainbowit.net/themes/inbio/cart/"
                ><span class="mini-cart"
                  ><i class="feather-shopping-cart"></i
                  ><span class="rbt-cart-count">0</span></span
                ></a
              >
            </div>
            <a class="rn-btn" href="#contacts"><span>CONTACT ME</span></a>

            <div class="hamberger-menu d-block d-xl-none">
              <i
                @click="menuOpen"
                id="menuBtn"
                class="feather-menu humberger-menu"
              ></i>
            </div>

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
import { menuItemsElementPages } from "~/data/menu";
import { menuOpen } from "~/utlis/menuToggle";
</script>

<style lang="scss" scoped></style>
