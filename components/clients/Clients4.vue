<template>
  <div
    class="row align-items-center justify-content-center sr-designer-clients"
  >
    <div
      v-for="(elm, i) in clients4"
      :key="i"
      class="col-lg-2 col-md-4 col-sm-6 sr-desiner-brand"
    >
      <nuxt-img :src="elm.imgSrc" alt="image" />
    </div>
  </div>
</template>

<script setup>
import { clients4 } from "~/data/clients";
</script>

<style lang="scss" scoped></style>
