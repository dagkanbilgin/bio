<template>
  <div style="color: aliceblue" v-if="!props.error.statusCode == 404">
    An error found with {{ props.error.statusCode }} status code
  </div>
  <div v-else class="template-color-1">
    <div class="error-area">
      <div class="container">
        <div class="row justify-content-center text-center">
          <div class="col-10">
            <h1 class="title">404!</h1>
            <h3 class="sub-title">Page not found</h3>
            <p>The page you were looking for could not be found.</p>
            <nuxt-link class="rn-btn" to="/"
              ><span>Back To Home</span></nuxt-link
            >
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const props = defineProps({
  error: Object,
});
const router = useRouter();

useSeoMeta({
  title: ` ${
    props.error.statusCode == 404 ? "Page not found" : "An error found"
  }  ||  Histudy - Online Courses & Education Vue 3 Nuxtjs Template.`,
  description: " Histudy - Online Courses & Education Vue 3 Nuxtjs Template.",
});
// if (props.error.statusCode == 404) {
//   router.push("/");
// }
</script>

<style lang="scss">
@import "./public/assets/css/vendor/bootstrap.min.css";

@import "./public/assets/scss/style.scss";
</style>
