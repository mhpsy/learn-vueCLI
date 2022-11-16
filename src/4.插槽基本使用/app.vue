<template>
  <div class="box">
    <user-slot>
      <div>{{ msg }}</div>
    </user-slot>
    <hr>

    <user-slot>
      <a href="#">{{ msg }}</a>
    </user-slot>
    <hr>

    <user-slot>
      <button>{{ msg }}</button>
    </user-slot>

    <hr>

    <user-slot>

    </user-slot>
  </div>
</template>

<script>
import userSlot from "@/4.插槽基本使用/components/userSlot";

export default {
  name: "app",
  components: {
    userSlot
  },

  data() {
    return {
      msg: 'test slot'
    }
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
