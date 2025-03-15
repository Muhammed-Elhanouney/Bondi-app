<template>
  <div class="main pt-5">
    <div class="container text-center">
      <TiltePage
        page-title="Some Stuff About Us"
        page-sub-title="The Great Team"
        :page-image="title"
      />
      <div class="hero-text">
        <p class="text-secondary">
          Donec rutrum congue leo eget malesuada. Mauris blandit aliquet elit,
          eget tincidunt nibh pulvinar a. Pellentesque in ipsum id orci porta
          dapibus. Proin eget tortor risus. Donec sollicitudin molestie
          malesuada.
        </p>
      </div>
      <div class="hero-one">
        <div class="row">
          <div class="col-12 col-lg-4 pb-5 text-sm-center text-lg-start">
            <h2>Retina Design</h2>
            <p>
              Vestibulum ac diam sit amet quam vehicula elementum sed sit amet
              dui. Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a.
              Donec rutrum congue leo eget malesuada. Mauris blandit aliquet
              elit, eget tincidunt nibh pulvinar a. Pellentesque in ipsum id
              orci porta dapibus. Proin eget tortor risus. Donec sollicitudin
              molestie malesuada.
            </p>
            <button class="btn d-none d-lg-block">order now</button>
          </div>
          <div class="col-12 col-lg-8">
            <img class="img-fluid" :src="lap" alt="" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import TiltePage from "./TiltePage.vue";

import title from "@/assets/imgs/title.png";
import lap from "@/assets/imgs/laptop.png";
</script>

<style lang="scss" scoped>
@use "@/assets/css/main.scss" as main;

.hero-text {
  margin: 50px auto;
  max-width: 500px;
  font-weight: bold;
}
.hero-one {
  position: relative;

  button {
    position: absolute;
    left: 0;
    background-color: main.$btn-color;
    color: main.$first-color;
    border-radius: 50px;
    text-transform: uppercase;
  }
}
</style>
