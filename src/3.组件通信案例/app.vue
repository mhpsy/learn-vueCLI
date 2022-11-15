<template>
  <div>
    <table-nav
        :procList="['手机','平板','电脑']"
        @tableNavClick="tableNavClick"
    ></table-nav>
    <div>
      {{ showData[currentIndex] }}
    </div>

  </div>
</template>

<script>
import tableNav from "@/3.组件通信案例/components/tableNav";

export default {
  components: {
    tableNav
  },
  name: "app",
  data() {
    return {
      currentIndex: 0,
      showData: ['手机内容', '平板内容', '电脑内容']
    }
  },
  create() {
  },
  mounted() {
  },
  computed() {
  },
  methods: {
    tableNavClick(index) {
      console.log('tableNavClick', index)
      this.currentIndex = index
    }
  }
}
</script>

<style scoped>

</style>
