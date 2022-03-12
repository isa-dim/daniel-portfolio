<template lang="pug">
div.q-ml-lg.circle.q-mb-xs(@click="show = !show")
transition
  div(v-if="show")
    div.q-ml-lg.circle-color.q-mb-xs
    div.q-ml-lg.circle-color-2.q-mb-xs
</template>
<script>
export default {
  name: 'ColorBtn',
  props: ['color'],
  data () {
    return {
      show: false
    }
  },
  methods: {
    changeColor () {
      console.log('hey')
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
  .circle:hover
    box-shadow: 0px 0px 5px 4px rgba(255,255,255,0.53)
    border: none
    cursor: pointer
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
  .v-enter-active,
  .v-leave-active
    transition: opacity 0.5s ease

  .v-enter-from,
  .v-leave-to
    opacity: 0
</style>
