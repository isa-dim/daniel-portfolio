<template lang="pug">
q-layout
  div.flex.test.window-height(:class="[$q.screen.lt.md ? 'column' : 'row']")
    div.left-item.full
      NaviMain
      h3.titulo.q-pa-lg(ref="text" @scroll="onScroll") Film student with a love for images & stories
    q-page-sticky(position="right").right-item
      div.window-height.width
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

export default defineComponent({
  name: 'PageIndex',
  components: { NaviMain, TableElement },
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
          year: '2021'
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
  top: 0
  background: white
  color: $dc-green
  // flex: 1
  width: 50%
.left-item
  width: 50%
  // flex: 1
.width
  width: 50vw
.full
  height: 4000px
.titulo
  max-width: 9.5em
</style>
