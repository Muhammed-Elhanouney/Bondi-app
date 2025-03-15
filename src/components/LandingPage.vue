<template>
  <div class="main-land">
    <div class="container text-center pt-5 pb-5">
      <h1 class="text-light text-capitalize">Taste the Creativity</h1>
      <p class="text-secondary">We make awesome graphic and web design</p>
      <button class="btn">get started</button>
    </div>
  </div>
</template>

<script>
export default {};
</script>
<style lang="scss" scoped>
@use "@/assets/css/main.scss" as main;

.main-land {
  background-color: main.$main-color;
  height: 500px;
  .container {
    top: 50%;
    transform: translateY(50%);
    .btn {
      border: none;
      background-color: main.$btn-color;
      padding: 10px;
      border-radius: 50px;
      color: main.$first-color;
      font-weight: bold;
      text-transform: capitalize;
    }
  }
}
</style>
