
<template>
  <table>
    <JTableRow
      v-for="(values, index) in items"
      :key="index"
      :values="values"
    />
  </table>
</template>

<script>
import JTableRow from '@rafael_dias/j-table-row/JTableRow'
export default {
  name: 'JTable',
  props: {
    items: {
      type: Array,
      required: true
    }
  },
  components: {
    JTableRow
  }
}
</script>