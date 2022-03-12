<template lang="pug">
div.row.test.window-height
  div.col-6
    NaviMain
    h3.titulo.q-pa-lg Film student with a love for images & stories
  div.right-item.col-6
    TableElement
</template>

<script>
import { defineComponent } from 'vue'
import NaviMain from 'components/NaviMain'
import TableElement from 'components/TableElement'

export default defineComponent({
  name: 'PageIndex',
  components: { NaviMain, TableElement }
})
</script>

<style media="screen" scoped lang="sass">
.right-item
  background: white
  color: $dc-green
.titulo
  max-width: 400px
</style>
