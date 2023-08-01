<template>
  <Ex335 :header="header" :rows="rows" />
</template>

<script>
import Ex335 from "./Ex335.vue";

export default {
  name: "Ex336",
  data() {
    return {
      header: ['1번 제목', '2번 제목'],
      rows: [
          [{data: '1번 내용'}, {data: '2번 내용'}],
          [{data: '1번 내용2', colspan: 2}],
      ],
    }
  },
  components: {
    Ex335,
  },
}
</script>

<style scoped>

</style>