<template>
  <div class="container">
    <img
      src="../../assets/background/big_circle_right.svg"
      class="big_circle_right"
    />
    <img
      src="../../assets/background/big_circle_left.svg"
      class="big_circle_left"
    />
    <div>
      <img
        src="../../assets/background/mid_circle_right.svg"
        class="mid_circle_right"
      />
      <img
        src="../../assets/background/small_circle_right.svg"
        class="small_circle_right"
      />
      <img src="../../assets/background/small_top.svg" class="small_top" />
    </div>
  </div>
</template>

<script>
export default {
  name: "loginPage",
};
</script>

<style scoped>
.big_circle_right {
  position: absolute;
  bottom: 0;
  right: 0;
}

.big_circle_left {
  position: absolute;
  top: 0;
  left: 0;
}

.mid_circle_right {
  position: absolute;
  right: 0;
  bottom: 45vh;
}

.small_circle_right {
  position: absolute;
  right: 10vw;
  bottom: 55vh;
}

.small_top {
  position: absolute;
  right: 13vw;
  bottom: 38vh;
}
</style>
