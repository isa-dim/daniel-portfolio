<template lang="pug">
div.circle.q-mb-xs
div.circle-color.q-mb-xs
div.circle-color-2.q-mb-xs
</template>
<script>
export default {
  name: 'ColorBtn',
  props: ['color'],
  data () {
    return {

    }
  }
}
</script>
<style lang="sass">
  .circle
    border-radius: 50%
    width: 20px
    height: 20px
    border: 1px solid white
  .circle-color
    border-radius: 50%
    width: 20px
    height: 20px
    background: pink
  .circle-color-2
    border-radius: 50%
    width: 20px
    height: 20px
    background: blue
</style>
