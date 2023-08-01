<template>
  <div style="width: 200px">
    <ol>
      <!--(값, 키, 인덱스) in 객체-->
      <li v-for="item in items">{{ item }}</li>
    </ol>
  </div>
</template>

<script>
import {reactive} from 'vue'

export default {
  name: "Ex311",
  setup() {
    const items = reactive(['1번 아이템','2번 아이템', '3번 아이템']);  //배열의 반응성을가지기 위함
    return {
      items,
    }
  }
}
</script>

<style scoped>

</style>