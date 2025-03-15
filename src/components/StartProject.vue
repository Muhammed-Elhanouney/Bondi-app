<template>
  <div class="main">
    <div class="container text-center">
      <h2>Start Your Project Now</h2>
      <p>
        Leave your description and we start the engine.Don't worry,you can
        cancel anytime
      </p>
      <button>start now</button>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "@/assets/css/main.scss" as main;

.main{
    padding: 100px 0;
    background-color: main.$main-color;

    h2{
        color: white;
    }
    p{
        color: #6a777b;
    }
    button{
        background-color: main.$btn-color;
        border: none;
        color: main.$first-color;
        border-radius: 50px;
        padding: 10px ;
        text-transform: uppercase;
        margin-top: 30px;
    }
}
</style>
