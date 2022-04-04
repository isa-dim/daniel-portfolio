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
      a.caudex-light.text-h5(href="mailto:info@daniel-cortes.com" target="_blank" rel="noopener noreferrer") info@daniel-cortes.com
    div.q-my-lg.flex.column
      p Portfolio
      a.caudex-light.text-h5(href="https://instagram.com/danielotecortes" target="_blank" rel="noopener noreferrer") Instagram
      a.caudex-light.text-h5(href="https://vimeo.com/user116307814" target="_blank" rel="noopener noreferrer") Vimeo
    q-img.q-my-xl(
      src="images/Daniel-Cortes-sw.jpeg"
      fit="cover"
      style="height: 350px; max-width: 20rem")
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
  overflow-y: scroll
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
  height: 15px
  width: 15px
  border-radius: 50px
  background-color: white
a
  color: $dc-green
a:hover
  text-decoration: underline
</style>
