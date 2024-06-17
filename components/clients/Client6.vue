<template>
  <div class="container rn-section-gap scrollSpysection" id="client">
    <div class="row mb--40">
      <div class="col-lg-12 text-center">
        <div class="section-title">
          <span class="subtitle">MY WORK HAS BEEN FEATURED ON:</span>
        </div>
      </div>
    </div>
    <div class="client-card client-card-2 sr-clients-2">
      <!-- Start Single Brand  -->
      <div v-for="(elm, i) in clients3" :key="i" class="main-content">
        <div class="inner text-center">
          <div class="thumbnail">
            <a :href="elm.href"><img :src="elm.src" alt="Client-image" /></a>
          </div>
        </div>
      </div>
      <!-- End Single Brand  -->
    </div>
  </div>
</template>

<script setup>
import { clients3 } from "~/data/clients";
</script>

<style lang="scss" scoped></style>
