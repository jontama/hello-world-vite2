<template>
  <p>{{ `[${msg}] : ${msg2}` }}</p>
  <Component v-model:msg="msg" v-model:msg2="msg2"/>
</template>

<script>
import Component from './Component.vue'
export default {
  name: "Ex318",
  data() {
    return {
      msg: '초기 메세지',
      msg2: '초기 메세지',
    }
  },
  Component: {
    Component,
  },
}
</script>

<style scoped>

</style>