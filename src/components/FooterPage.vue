<script setup>
import logo from "@/assets/imgs/logo.png";
import BtnPage from "./BtnPAge.vue";
</script>

<template>
  <div class="main">
    <div class="container text-center">
      <div class="row">
        <div class="col-12 col-md-6 col-lg-3">
          <img class="img-fluid" :src="logo" alt="" />
          <p class="text-secondary fw-bold mt-3">
            Pellentesque in ipsum id orci porta dapibus. Vivamus magna justo,
            lacinia eget consectetur sed, convallis at tellus.
          </p>
          <p class="text-secondary">
            Created By <span class="text-info">Graphberry</span> © 2022 -
            <span class="text-warning">Bondi Inc</span>
          </p>
        </div>
        <div class="col-12 col-md-6 col-lg-3">
          <h4 class="text-white">Links</h4>
          <ul class="text-secondary list-unstyled">
            <li>Home</li>
            <li>Our Services</li>
            <li>Portfolio</li>
            <li>Testimonials</li>
            <li>Support</li>
            <li>Terms and</li>
            <li>Condition</li>
          </ul>
        </div>
        <div class="col-12 col-md-6 col-lg-3">
          <h4 class="text-white">About Us</h4>
          <ul class="text-secondary list-unstyled">
            <li>Sign In</li>
            <li>Register</li>
            <li>About Us</li>
            <li>Blog</li>
            <li>Contact Us</li>
          </ul>
        </div>
        <div class="col-12 col-md-6 col-lg-3">
          <h4 class="text-white">Contact Us</h4>
          <p class="text-secondary">
            Get in touch with us via mail phone.We are waiting for your call or
            message
          </p>
          <btn-page title-btn="graphberry@gmail.com" />
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "@/assets/css/main.scss" as main;

.main {
  background-color: main.$main-color;
  padding: 50px 0;
}
</style>
