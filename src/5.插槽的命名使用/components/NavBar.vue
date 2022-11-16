<template>
  <div class="box">
    <div class="left">
      <slot name="left"></slot>
    </div>
    <div class="center">
      <slot name="center"></slot>
    </div>
    <div class="right">
      <slot name="right"></slot>
    </div>
  </div>
</template>

<script>

export default {
  name: "NavBar",
  data() {
    return {}
  },
  create() {
  },
  mounted() {
  },
  computed() {
  },
  methods: {}
}
</script>

<style scoped>
.box {
  display: flex;
  justify-content: space-between;
}

.left, .center, .right {
  height: 44px;
  text-align: center;
  /*line-height: 44px;*/
  display: flex;
  align-items: center;
  justify-content: space-around;

}

.left {
  width: 80px;
  background-color: antiquewhite;
}

.center {
  flex: 1;
  background-color: beige;
}

.right {
  width: 80px;
  background-color: cyan;
}
</style>
