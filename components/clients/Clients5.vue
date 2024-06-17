<template>
  <div
    class="container px-0 row rn-section-gap-2 align-items-center justify-content-center mx-auto client-5"
  >
    <div
      v-for="(elm, i) in clients5"
      :key="i"
      class="col-lg-2 col-md-4 col-sm-6 sr-desiner-brand"
    >
      <img :src="elm.imgSrc" alt="image" />
    </div>
  </div>
</template>

<script setup>
import { clients5 } from "~/data/clients";
</script>

<style lang="scss" scoped></style>
