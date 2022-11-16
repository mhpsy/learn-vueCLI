<template>
  <div class="box">
    <slot>
      <div>我是slot的默认值</div>
    </slot>
  </div>
</template>

<script>

export default {
  name: "userSlot",
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
