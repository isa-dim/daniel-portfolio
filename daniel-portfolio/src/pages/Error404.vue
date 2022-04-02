<template lang="pug">
div.row
  div.col-md-6.col-12
    div.left
  div.col-md-6.col-12
    div.right
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'Error404'
})
</script>

<style lang="sass">
.left
  background-color: red
.right
  background-color: blue
</style>
