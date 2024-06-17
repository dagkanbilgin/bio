<template>
  <CommonMobileMenu :navItems="navItemsHomeConsulting" />
  <div class="header-style-2 d-block d-xl-none">
    <div class="row align-items-center">
      <div class="col-6">
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
      <div class="col-6">
        <div class="header-right text-end">
          <div class="hamberger-menu">
            <i
              id="menuBtn"
              class="feather-menu humberger-menu"
              @click="menuOpen"
            ></i>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="d-none d-xl-block">
    <header
      class="rn-header-area d-flex align-items-start flex-column left-header-style"
    >
      <div class="logo-area">
        <nuxt-link to="/">
          <nuxt-img src="/assets/images/logo/logo-06.png" alt="personal-logo" />
        </nuxt-link>
      </div>
      <nav id="sideNavs" class="mainmenu-nav navbar-example2 onepagenav">
        <ul class="primary-menu nav nav-pills scrollspyLinks">
          <li
            v-for="(elm, i) in navItemsHomeConsulting"
            :key="i"
            :class="`nav-item ${!i ? 'current' : ''} `"
          >
            <a class="nav-link smoth-animation-two" :href="elm.href"
              ><i :data-feather="elm.icon"></i> {{ elm.title }}</a
            >
          </li>
        </ul>
      </nav>
      <div class="footer">
        <div class="rbt-mini-cart-wrap">
          <a href="#"
            ><span class="mini-cart"
              ><i class="feather-shopping-cart"></i
              ><span class="rbt-cart-count">0</span></span
            ></a
          >
        </div>
        <div class="social-share-style-1 mt--40">
          <span class="title">find with me</span>
          <ul class="social-share d-flex liststyle">
            <li class="facebook">
              <a href="#"
                ><svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  class="feather feather-facebook"
                >
                  <path
                    d="M18 2h-3a5 5 0 0 0-5 5v3H7v4h3v8h4v-8h3l1-4h-4V7a1 1 0 0 1 1-1h3z"
                  ></path></svg
              ></a>
            </li>
            <li class="instagram">
              <a href="#"
                ><svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  class="feather feather-instagram"
                >
                  <rect x="2" y="2" width="20" height="20" rx="5" ry="5"></rect>
                  <path
                    d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"
                  ></path>
                  <line x1="17.5" y1="6.5" x2="17.51" y2="6.5"></line></svg
              ></a>
            </li>
            <li class="linkedin">
              <a href="#"
                ><svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  class="feather feather-linkedin"
                >
                  <path
                    d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"
                  ></path>
                  <rect x="2" y="9" width="4" height="12"></rect>
                  <circle cx="4" cy="4" r="2"></circle></svg
              ></a>
            </li>
          </ul>
        </div>
      </div>
    </header>
  </div>
</template>

<script setup>
import { navItemsHomeConsulting } from "~/data/menu";
import addScrollspy from "~/utlis/addScrollSpy";
import addSmoothScroll from "~/utlis/addSmoothScroll";
import { menuOpen } from "~/utlis/menuToggle";

defineProps(["navItems"]);
function ititScrollspy() {
  addScrollspy("nav-link smoth-animation-two");
}
onMounted(() => {
  addSmoothScroll();
  window.addEventListener("scroll", ititScrollspy);
});
onUnmounted(() => {
  window.removeEventListener("scroll", ititScrollspy);
});
</script>

<style lang="scss" scoped></style>
