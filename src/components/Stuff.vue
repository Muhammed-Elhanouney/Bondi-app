<template>
  <div class="main pt-5 pb-5">
    <div class="container text-center">
      <tilte-page
        page-title="We are Good at"
        page-sub-title="Some Of These Stuff Under"
        :page-image="title"
      />

      <div class="hero-stuff">
        <div class="row">
          <div class="col-12 col-md-6 col-lg-4 text-center p-4">
            <span class="pt-5">
              <i class="fa-solid back fa-1"></i>
              <i class="fa-solid front fa-pencil"> </i
            ></span>
            <h3>Graphic Design</h3>
            <p>
              Pellentesque in ipsum id orci porta dapibus. Vivamus magna justo,
              lacinia eget consectetur sed, convallis at tellus.
            </p>
          </div>
          <div class="col-12 col-md-6 col-lg-4 text-center p-4">
            <span>
              <i class="fa-solid back fa-2"></i>
              <i class="fa-solid front fa-tv"></i>
            </span>
            <h3>Graphic Design</h3>
            <p>
              Pellentesque in ipsum id orci porta dapibus. Vivamus magna justo,
              lacinia eget consectetur sed, convallis at tellus.
            </p>
          </div>
          <div class="col-12 col-md-6 col-lg-4 text-center p-4">
            <span>
              <i class="fa-solid back fa-3"></i>
              <i class="fa-solid front fa-plug"></i>
            </span>
            <h3>Graphic Design</h3>
            <p>
              Pellentesque in ipsum id orci porta dapibus. Vivamus magna justo,
              lacinia eget consectetur sed, convallis at tellus.
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import title from "@/assets/imgs/title.png";
import TiltePage from "./TiltePage.vue";
</script>

<style lang="scss" scoped>
@use "@/assets/css/main.scss" as main;

.hero-stuff {
  margin-top: 100px;
  span {
    position: relative;
    .back {
      color: main.$second-color;
      position: absolute;
      opacity: 0.2;
      bottom: 0;
      font-size: 6rem;
      left: 50%;
      transform: translateX(-50%);
    }
    .front {
      color: main.$second-color;
      font-size: 3rem;
      padding-bottom: 40px;
    }
  }
  h3 {
    color: main.$first-color;
  }
  p {
    font-weight: bold;
  }
}
</style>
