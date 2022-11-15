<template>
  <div class="box">
    <div v-for="(item,index) in procList"
         class="box-show-item"
         @click="itemClick(index)"
         :class="{active:index===currentIndex}"
    >
      <span>{{ item }}</span>
    </div>
  </div>
</template>

<script>

export default {
  props: {
    procList: {
      type: Array,
      default: () => []
    },
  },
  name: "tableNav",
  data() {
    return {
      currentIndex: 0
    }
  },
  create() {
  },
  mounted() {
  },
  computed() {
  },
  methods: {
    itemClick(index) {
      this.currentIndex = index
      this.$emit('tableNavClick', index)
    }
  }
}
</script>

<style scoped>
.box {
  display: flex;
}

.box-show-item {
  flex: 1;
  text-align: center;
  font-size: 30px;
}

.box-show-item.active {
  color: red;
}

.box-show-item.active span {
  border-bottom: red solid 3px;
  padding: 5px 10px;
}

</style>
