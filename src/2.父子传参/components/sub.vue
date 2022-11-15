<template>
  <div>
    <button v-for="num in numbers" @click="btnClick(num)">-{{ num }}</button>
  </div>
</template>

<script>

export default {
  props: {
    numbers: {
      type: Array,
      default: () => [1, 2, 3]
    }
  },
  name: "sub",
  data() {
    return {}
  },
  create() {
  },
  mounted() {
  },
  computed() {
  },
  methods: {
    btnClick(num) {
      this.$emit("sub", num)
    }
  }
}
</script>

<style scoped>

</style>
