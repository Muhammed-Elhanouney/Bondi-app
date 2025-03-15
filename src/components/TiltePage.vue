<template>
  <div class="good">
    <img :src="pageImage" alt="" />
    <h3 class="mt-3 text-dark text-capitalize">{{ pageTitle }}</h3>
    <p class="text-secondary text-uppercase add-text">
      {{ pageSubTitle }}
    </p>
  </div>
</template>

<script>
export default {
  props: {
    pageTitle: String,
    pageSubTitle: String,
    pageImage: String,
  },
};
</script>

<style lang="scss" scoped>
.add-text {
  position: relative;
  &::after {
    position: absolute;
    content: "";
    left: 50%;
    transform: translateX(-50%);
    bottom: -20px;
    width: 10%;
    height: 3px;
    background-color: aqua;
    border-radius: 50px;
  }
}
</style>
