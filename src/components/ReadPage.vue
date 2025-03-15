<script setup>
import title from "@/assets/imgs/title.png";
import blog1 from "@/assets/imgs/blog-1.jpg";
import blog2 from "@/assets/imgs/blog-2.jpg";
import blog3 from "@/assets/imgs/blog-3.jpg";
import TiltePageVue from "./TiltePage.vue";
</script>

<template>
  <div class="main">
    <div class="container text-center">
      <TiltePageVue
        pageTitle="Read Our Blog"
        pageSubTitle="New Stories"
        :pageImage="title"
      />
      <div class="hero-box">
        <div class="row">
          <div class="col-12 col-md-6 col-lg-4 p-sm-2">
            <div class="box">
              <img class="img-fluid" :src="blog1" alt="" />
              <p>Jan 17, 2022</p>
              <h4>Some Awesome Blog Title Here</h4>
            </div>
          </div>
          <div class="col-12 col-md-6 col-lg-4 p-sm-2">
            <div class="box">
              <img class="img-fluid" :src="blog2" alt="" />
              <p>Jan 17, 2022</p>
              <h4>Some Awesome Blog Title Here</h4>
            </div>
          </div>
          <div class="col-12 col-md-6 col-lg-4 p-sm-2">
            <div class="box">
              <img class="img-fluid" :src="blog3" alt="" />
              <p>Jan 17, 2022</p>
              <h4>Some Awesome Blog Title Here</h4>
            </div>
          </div>
        </div>
        <button>more stories</button>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "@/assets/css/main.scss" as main;

.main {
  padding: 100px 0;
}

.hero-box {
  padding: 50px 0;
  .box {
    border-radius: 20px;
    overflow: hidden;
    text-align: start;
    border: solid 2px #eee;
    p {
      margin-top: 20px;
      padding: 0 10px;
    }
    h4 {
      padding: 0 10px;
    }
  }
  button {
    margin-top: 40px;
    background-color: main.$btn-color;
    border: none;
    color: main.$first-color;
    border-radius: 50px;
    padding: 10px;
    text-transform: uppercase;
  }
}
</style>
