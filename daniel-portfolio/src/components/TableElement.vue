<template lang="pug">
div.q-mx-lg
  div.table-style.flex.justify-between.border.q-pt-md.mono.positioning
    p {{ title }}
    p {{ category }}
    p {{ year }}
</template>

<script>
export default {
  name: 'TableElement',
  props: ['title', 'category', 'year']
}
</script>

<style lang="sass" scoped>
.border
  border-top: 1px solid $dc-green
.mono
  font-family: IBMPlexMono-Regular
  font-size: .7rem
.positioning
  position: absolute
  bottom: 0
.table-style
  width: 95%
</style>
