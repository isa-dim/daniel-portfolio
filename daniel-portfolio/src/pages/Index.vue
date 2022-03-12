<template lang="pug">
div.row.test.window-height
  div.col-6
    p daniel cortes
  div.right-item.col-6
    p isabela
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'PageIndex'
})
</script>

<style media="screen" scoped lang="sass">
.right-item
  background: white
  color: $dc-green
</style>
