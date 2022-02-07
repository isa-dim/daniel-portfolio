<template lang="pug">
div.q-ma-lg.q-pt-lg(:class="[$q.screen.lt.md ? 'q-mb-md' : 'max-width']")
  h5.q-pb-lg I'm Daniel Cortés, a Germany based graphic designer and developer working on projects in fields ranging from identity, print, editorial design and art direction to websites and interactive design for businesses, individuals and cultural institutions.
  h5 Please contact me if you'd like to discuss a project.
  div.q-mb-lg(v-for="item in infos")
    p {{ item.title }}
    h5 {{ item.body }}
  q-img.q-my-xl(
    src="images/Daniel-Cortes-sw.jpeg"
    fit="cover"
    style="max-width: 400px")
</template>

<script>
export default {
  name: 'About',
  data () {
    return {
      infos: {
        main: {
          title: '',
          body: ''
        },
        email: {
          title: 'E-Mail',
          body: 'info@daniel-cortes.com'
        },
        social: {
          title: 'Social Media',
          body: 'Instagram',
          body2: 'Vimeo'
        }
      }
    }
  }
}
</script>

<style lang="sass" scoped>
.max-width
    max-width: 50%
</style>
