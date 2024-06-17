<template>
  <div class="rn-footer-area rn-section-gap section-separator mw-100">
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <div class="footer-area text-center">
            <div class="logo">
              <nuxt-link to="/">
                <nuxt-img
                  :width="59"
                  :height="85"
                  class="logo-light"
                  src="/assets/images/logo/logo-vertical.png"
                  alt="logo"
                />
                <nuxt-img
                  :width="59"
                  :height="85"
                  class="logo-dark"
                  src="/assets/images/logo/logo-vertical-dark.png"
                  alt="logo"
                />
              </nuxt-link>
            </div>

            <p class="description mt--30">
              © {{ new Date().getFullYear() }}. All rights reserved by
              <a
                target="_blank"
                href="https://themeforest.net/user/rainbow-themes/portfolio"
                >Rainbow-Themes.</a
              >
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped></style>
