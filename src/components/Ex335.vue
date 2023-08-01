<template>
  <table>
    <tr>
      <th v-for="(head, head_index) in header" :key="'head-' + head_index">
        {{ head }}
      </th>
    </tr>
    <tr v-for="(rows, row_index) in rows" :key="'row-' + row_index">
      <td v-for="(data, data_index) in rows" :key="'data-' + data_index" :colspan="data.colspan || 1">
        {{ data.data }}
      </td>
    </tr>
  </table>

</template>

<script>
//EX336 부속

export default {
  name: "Ex335",
  props: ['header', 'rows'],
}
</script>

<style scoped>
table,
th,
td {
  border: 1px solid black;
  borser-collapse: collapse;
  padding: 5px;
}

</style>