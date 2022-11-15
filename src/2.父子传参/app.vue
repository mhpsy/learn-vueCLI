<template>
  <add @add="addClick" :numbers="numbers"></add>
  <h2>{{ count }}</h2>
  <subNum @sub="subClick" :numbers="[3,5,8]"></subNum>
  <!--   Do not use built-in or reserved HTML elements as component id: sub -->
</template>

<script>
import add from "@/2.父子传参/components/add";
import sub from "@/2.父子传参/components/sub"

export default {
  components: {
    add,
    subNum: sub
    //   Do not use built-in or reserved HTML elements as component id: sub
  },
  name: "sub",
  data() {
    return {
      count: 10,
      numbers: [1, 5, 10],
    }
  },
  create() {
  },
  mounted() {
  },
  computed() {
  },
  methods: {
    subClick(num) {
      this.count -= num
    },
    addClick(num) {
      this.count += num
    }
  }
}
</script>

<style scoped>

</style>
