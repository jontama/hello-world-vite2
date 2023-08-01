<template>
  <p>{{ counter }}</p>
  <p v-if="counter < 5">5 보다 작습니다.</p>
  <p v-else>5와 같거나 큽니다.</p>
  <button @click="counter++">클릭하면 숫자가 올라갑니다.</button>
</template>

<script>
import { ref } from 'vue'

export default {
  name: "Ex310",
  setup() {
    let counter = ref(0)
    return {
      counter,
    }
  }
}
</script>

<style scoped>

</style>