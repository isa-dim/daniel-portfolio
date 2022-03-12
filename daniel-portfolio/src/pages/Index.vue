<template lang="pug">
div.flex.test.window-height(:class="[$q.screen.lt.md ? 'column' : 'row']")
  div.left-item
    NaviMain
    h3.titulo.q-pa-lg Film student with a love for images & stories
  div.right-item.window-height
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

<style  scoped lang="sass">
.right-item
  background: white
  color: $dc-green
  flex: 1

.left-item
  flex: 1

// .right-item
//     body.screen--xs &
//       visibility: hidden
.titulo
  max-width: 9.5em
</style>
