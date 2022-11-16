<template>
  <nav-bar>
    <template v-slot:left>
      <button>return</button>
    </template>

    <template #center>
      <div>首页的标题</div>
    </template>

    <template #right>
      <a href="#">登录</a>
    </template>
  </nav-bar>
</template>

<script>
import navBar from "@/5.插槽的命名使用/components/NavBar";

export default {
  components: {
    navBar
  },
  name: "app",
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

</style>
