<template>
  <div class="main">
    <div class="container text-center">
      <div class="row">
        <div class="col-12 col-sm-6 col-md-4 col-lg-2 p-3">
          <img :src="tech1" alt="" />
        </div>
        <div class="col-12 col-sm-6 col-md-4 col-lg-2 p-3">
          <img :src="tech2" alt="" />
        </div>
        <div class="col-12 col-sm-6 col-md-4 col-lg-2 p-3">
          <img :src="tech3" alt="" />
        </div>
        <div class="col-12 col-sm-6 col-md-4 col-lg-2 p-3">
          <img :src="tech4" alt="" />
        </div>
        <div class="col-12 col-sm-6 col-md-4 col-lg-2 p-3">
          <img :src="tech1" alt="" />
        </div>
        <div class="col-12 col-sm-6 col-md-4 col-lg-2 p-3">
          <img :src="tech2" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import tech1 from "@/assets/imgs/tech-1.png";
import tech2 from "@/assets/imgs/tech-2.png";
import tech3 from "@/assets/imgs/tech-3.png";
import tech4 from "@/assets/imgs/tech-4.png";
</script>

<style lang="scss" scoped>
@use "@/assets/css/main.scss" as main;
.main {
  padding: 100px 0;
}
</style>
