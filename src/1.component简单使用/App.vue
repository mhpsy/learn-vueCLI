<template>
  <div>
    <show-info v-for="item in showDate"
               :name="item.name"
               :age="item.age"
               :sex="item.sex"
    ></show-info>
  </div>
</template>

<script>
import showInfo from "@/1.component简单使用/components/showInfo";

export default {
  name: 'App',
  components: {
    showInfo
  },
  data() {
    return {
      showDate: [
        {
          name: 'xx',
          age: 20,
          sex: 'man'
        },
        {
          name: 'xxx',
          age: 21,
          sex: 'man'
        },
        {
          name:'aa'
        }
      ]
    }
  }
}
</script>

<style>

</style>
