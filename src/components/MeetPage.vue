<template>
  <div class="main">
    <div class="container text-center">
      <div class="hero-text">
        <h2>Meet The Team</h2>
        <p>
          Donec rutrum congue leo eget malesuada. Mauris blandit aliquet elit,
          eget tincidunt nibh pulvinar a. Pellentesque in ipsum id orci porta
          dapibus. Proin eget tortor risus. Donec sollicitudin molestie
          malesuada.
        </p>
      </div>
      <div class="hero-box ">
        <div class="row">
          <div class="col-12 col-sm-6 col-md-4 col-lg-3">
            <div class="box">
              <img class="img-fluid" :src="team1" alt="" />
              <h3>Luke Skywalker </h3>
              <p>
                “I don't understand how we got by those troops. I thought we
                were dead.“
              </p>
            </div>
          </div>
          <div class="col-12 col-sm-6 col-md-4 col-lg-3">
            <div class="box">
              <img class="img-fluid" :src="team2" alt="" />
              <h3>Luke Skywalker </h3>
              <p>
                “I don't understand how we got by those troops. I thought we
                were dead.“
              </p>
            </div>
          </div>
          <div class="col-12 col-sm-6 col-md-4 col-lg-3">
            <div class="box">
              <img class="img-fluid" :src="team3" alt="" />
              <h3>Luke Skywalker </h3>
              <p>
                “I don't understand how we got by those troops. I thought we
                were dead.“
              </p>
            </div>
          </div>
          <div class="col-12 col-sm-6 col-md-4 col-lg-3">
            <div class="box">
              <img class="img-fluid" :src="team4" alt="" />
              <h3>Luke Skywalker </h3>
              <p>
                “I don't understand how we got by those troops. I thought we
                were dead.“
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import team1 from "@/assets/imgs/team-1.png";
import team2 from "@/assets/imgs/team-2.png";
import team3 from "@/assets/imgs/team-3.png";
import team4 from "@/assets/imgs/team-4.png";
</script>

<style lang="scss" scoped>
@use "@/assets/css/main.scss" as main;
.main {
  background-color: main.$section-color;
  padding: 100px;
  .hero-text {
    h2 {
      color: main.$first-color;
      font-weight: bold;
    }
    p {
      color: #6a777b;
    }
  }
  .hero-box {
    margin-top: 20px;
    .box {
      h3 {
        background-color: aqua;
        padding: 10px;
        margin: 0;
        color: white;
      }
      p {
        background-color: white;
        color: #6a777b;
        padding: 20px 12px;
      }
    }
  }
}
</style>
