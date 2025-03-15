<template>
  <button>{{ titleBtn }}</button>
</template>

<script>
export default {
  props: {
    titleBtn: String,
  },
};
</script>

<style lang="scss" scoped>
@use "@/assets/css/main.scss" as main;

button {
  border: none;
font-weight: bold;
padding: 10px 20px;
  text-transform: uppercase;
  color: main.$first-color;
  background-color: main.$btn-color;
  border-radius: 50px;
}
</style>
