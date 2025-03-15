<template>
  <nav class="navbar navbar-expand-lg bg-body-black ">
    <div class="container">
      <a class="navbar-brand" href="#">
        <img :src="logo" alt="" />
      </a>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">Home</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">about</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Srvices</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Portfolio</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Contact Us</a>
          </li>
        </ul>
        <div class="end d-none d-lg-block">
          <span><i class="fa-solid fa-magnifying-glass"></i></span>
          <button >Log In</button>
        </div>
      </div>
    </div>
  </nav>
</template>

<script setup>
import logo from "@/assets/imgs/logo.png";
</script>

<style lang="scss" scoped>
@use "@/assets/css/main.scss" as main;

nav {
  background-color: main.$main-color;
  .active {
    color: main.$second-color !important;
  }
  .navbar-toggler
  {
      background-color: white !important;
      border: solid 1px white;
  }
  .nav-link {
    color: white;
    font-weight: bold;
    &:hover,
    &:focus {
      color: main.$second-color;
    }
  }

  .end {
    span {
      position: relative;
      color: main.$second-color;
      padding: 0 30px;

      &::before {
        content: "";
        width: 1px;
        height: 35px;
        position: absolute;
        background-color: main.$second-color;
        left: 10px;
        top: 50%;
        transform: translateY(-50%);
      }
    }
    button {
      border: none;
      background-color: main.$btn-color;
      padding: 10px;
      border-radius: 50px;
      color: main.$first-color;
      font-weight: bold;
    }
  }
}
</style>
