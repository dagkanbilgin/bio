<template>
  <div class="rn-skill-area section-height scrollSpysection" id="skill">
    <div class="inner slide">
      <h5 class="title">About My Skill</h5>
      <div class="skill-share-inner pt--100">
        <span class="title">Primary Skills on</span>
        <ul class="skill-share d-flex liststyle">
          <li v-for="(elm, i) in primarySkills" :key="i">
            <nuxt-img :src="elm.src" alt="Icons Images" />
          </li>
        </ul>
      </div>
      <div class="skill-share-inner skill-share-inner-width margin-top-25">
        <span class="title">Secondary Skills on</span>
        <ul class="skill-share d-flex liststyle">
          <li v-for="(elm, i) in secondarySkills" :key="i">
            <nuxt-img :src="elm.src" alt="Icons Images" />
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script setup>
import { primarySkills, secondarySkills } from "~/data/skills";
</script>

<style lang="scss" scoped></style>
