<template>
  <div class="main">
    <div class="container text-center">
      <tilte-page
        page-title="We Make This"
        page-sub-title="Prepare To Be Amazed"
        :page-image="title"
      />
      <div class="links">
        <ul class="list-unstyled">
          <li class="active">all</li>
          <li>design</li>
          <li>code</li>
          <li>photo</li>
          <li>app</li>
        </ul>
      </div>
      <div class="hero-img">
        <div class="row g-3">
          <div class="col-12 col-sm-6 col-md-4 col-lg-3">
            <div class="box" data-work="Appliction">
              <img class="img-fluid" :src="work1" alt="" />
            </div>
          </div>
          <div class="col-12 col-sm-6 col-md-4 col-lg-3">
            <div class="box" data-work="Appliction">
              <img class="img-fluid" :src="work2" alt="" />
            </div>
          </div>
          <div class="col-12 col-sm-6 col-md-4 col-lg-3">
            <div class="box" data-work="Appliction">
              <img class="img-fluid" :src="work3" alt="" />
            </div>
          </div>
          <div class="col-12 col-sm-6 col-md-4 col-lg-3">
            <div class="box" data-work="Appliction">
              <img class="img-fluid" :src="work4" alt="" />
            </div>
          </div>
          <div class="col-12 col-sm-6 col-md-4 col-lg-3">
            <div class="box" data-work="Appliction">
              <img class="img-fluid" :src="work5" alt="" />
            </div>
          </div>
          <div class="col-12 col-sm-6 col-md-4 col-lg-3">
            <div class="box" data-work="Appliction">
              <img class="img-fluid" :src="work6" alt="" />
            </div>
          </div>
          <div class="col-12 col-sm-6 col-md-4 col-lg-3">
            <div class="box" data-work="Appliction">
              <img class="img-fluid" :src="work7" alt="" />
            </div>
          </div>
          <div class="col-12 col-sm-6 col-md-4 col-lg-3">
            <div class="box" data-work="Appliction">
              <img class="img-fluid" :src="work8" alt="" />
            </div>
          </div>
        </div>
      </div>
      <div>
        <button class="btn">i want more</button>
      </div>
    </div>
  </div>
</template>

<script setup>
import TiltePage from "./TiltePage.vue";

import title from "@/assets/imgs/title.png";
import work1 from "@/assets/imgs/work-01.jpg";
import work2 from "@/assets/imgs/work-02.jpg";
import work3 from "@/assets/imgs/work-03.jpg";
import work4 from "@/assets/imgs/work-04.jpg";
import work5 from "@/assets/imgs/work-05.jpg";
import work6 from "@/assets/imgs/work-06.jpg";
import work7 from "@/assets/imgs/work-07.jpg";
import work8 from "@/assets/imgs/work-08.jpg";
</script>

<style lang="scss" scoped>
@use "@/assets/css/main.scss" as main;

.main {
  background-color: main.$section-color;
  padding: 50px 0;
}

.links {
  padding: 40px;
  ul {
    display: flex;
    justify-content: center;
    align-items: center;
    li {
      margin-left: 10px;
      padding: 5px 10px;
      cursor: pointer;
      text-transform: capitalize;
      font-weight: bold;

      &:hover,
      &:focus {
        color: main.$btn-color;
      }
    }
    .active {
      background-color: main.$btn-color;
      color: main.$first-color;
      border-radius: 50px;
      &:hover {
        color: white;
      }
    }
  }
}
.box {
  overflow: hidden;
  position: relative;

  &::before {
    content: attr(data-work);
    position: absolute;
    background-color: #33d1ccc7;
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    transform: translateX(calc(-100% - 5px));
    transition: 0.3s;
    color: white;
    gap: 10;
  }
  &:hover::before {
    transform: translateX(0);
  }
}
.btn {
  margin-top: 30px;
  text-transform: uppercase;
  color: main.$first-color;
  background-color: main.$btn-color;
  border-radius: 50px;
}
</style>
