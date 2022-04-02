<template lang="pug">
//left container
div.left-item.flex.column.caudex
  p.q-mt-lg Daniel Cortés
  h3.titulo Film student with a love for images & stories
  div.q-mb-lg.circle-filled
//right container
div.right-item.window-height
  div.sticky.q-ma-lg
    h5.caudex-light.q-pb-lg I'm Daniel Cortés, a Germany based Colombian film student with a love for documentary, images & stories of all kinds. Currently looking for an internship or a job opportunity.
    h5.caudex-light Please contact me if you'd like to discuss a project.
    div.q-my-lg
      p E-Mail
      h5.caudex-light info@danielcortes.com
    div.q-my-lg
      p Portfolio
      h5.caudex-light Instagram
    q-img.q-my-xl(
      src="images/Daniel-Cortes-sw.jpeg"
      fit="cover"
      style="height: 250px; max-width: 20rem")
</template>

<script>
import { defineComponent } from 'vue'
import NaviMain from 'components/NaviMain'
import TableElement from 'components/TableElement'
import ColorBtn from 'components/ColorBtn'
import DcImage from 'components/DcImage'

export default defineComponent({
  name: 'Temp',
  components: { NaviMain, TableElement, ColorBtn, DcImage },
  methods: {
    onScroll () {
      console.log('hey')
    }
  }
})
</script>

<style  scoped lang="sass">
.right-item
  background: white
  color: $dc-green
  flex: 1
  position: fixed
  z-index: 1
  top: 0
  right: 0
  height: 100vh
  width: 50%
.left-item
  width: 50%
  flex: 1
  height: 100vh
  display: flex
  align-items: center
  justify-content: space-between
.sticky-mobile
  width: 100vh
.titulo
  max-width: 25rem
  text-align: center
.caudex
  font-family: Caudex
.caudex-light
  font-family: Caudex
  font-weight: 200
.border
  border: 1px solid red
.circle-filled
  height: 20px
  width: 20px
  border-radius: 50px
  background-color: white
</style>
