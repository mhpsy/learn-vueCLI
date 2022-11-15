<template>
  <div>name：{{ name }}</div>
  <div>age：{{ age }}</div>
  <div>sex：{{ sex }}</div>
  <ul v-for="item in friend">
    <li>{{ item.name }}</li>
    <li>{{ item.address }}</li>
  </ul>
  <hr>
</template>

<script>

export default {
  name: "info",
  props: {
    name: {
      type: String,
      required: true,
    },
    age: {
      type: [String, Number],
      default: '20',
    },
    sex: {
      type: String,
      default: 'man',
    },
    friend: {
      //如果是对象的形式那么默认值必须是一个函数
      type: Object,
      default: () => [
        {name: 'xx', address: 'US'},
        {name: 'xxx', address: 'UK'},
      ]
    }
  },


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
