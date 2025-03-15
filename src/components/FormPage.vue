<script setup></script>
<template>
  <div class="main">
    <div class="container text-center">
      <form class="d-lg-flex justify-content-between" action="">
        <h4 class="mt-4">Subscribe to our Newsletter:</h4>
        <input
          type="text"
          placeholder="Enter Email Address Here"
          name="Email"
        />
        <div class="mt-4">
          <button>subscripe</button>
        </div>
      </form>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "@/assets/css/main.scss" as main;
.main {
  padding: 100px 0;
  background-color: main.$first-color;
  form {
  
    input {
      width: 50%;
      border: none;
      color: white;
      background-color: main.$first-color;
      outline: none;
      border-bottom: solid 1px white;
      &::placeholder{
        color: white;
      }
    }
    button {
      background-color: main.$main-color;
      border: none;
      padding: 10px 20px;
      border-radius: 50px;
      color: main.$first-color;
    }
  }
}
</style>
