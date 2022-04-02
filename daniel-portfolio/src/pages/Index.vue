<template lang="pug">
div.flex.test.window-height(:class="[$q.screen.lt.md ? 'column' : 'row']")
  div.left-item.full
    NaviMain
    h3.titulo.q-pa-lg(ref="text" @scroll="onScroll") Film student with a love for images & stories
    ColorBtn
    DcImage
  div.right-item.window-height
    div.sticky
      TableElement(
        v-for="project in projects"
        :title="project.title"
        :category="project.category"
        :year="project.year"
        )
</template>

<script>
import { defineComponent } from 'vue'
import NaviMain from 'components/NaviMain'
import TableElement from 'components/TableElement'
import ColorBtn from 'components/ColorBtn'
import DcImage from 'components/DcImage'

export default defineComponent({
  name: 'PageIndex',
  components: { NaviMain, TableElement, ColorBtn, DcImage },
  methods: {
    onScroll () {
      console.log('hey')
    }
  },
  data () {
    return {
      projects: [
        {
          title: 'Spain',
          category: 'Photography Series',
          year: '2020'
        },
        {
          title: 'Portraits',
          category: 'Photography Series',
          year: '2020'
        },
        {
          title: 'Aquí',
          category: 'Short Film',
          year: '2019'
        }
      ]
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
  flex: 1
.full
  // height: 4000px
.titulo
  max-width: 9.5em
</style>
