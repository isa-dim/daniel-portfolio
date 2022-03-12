<template lang="pug">
NaviDesktop
div.q-ma-lg.q-pt-lg(:class="[$q.screen.lt.md ? 'q-mb-md' : 'max-width']")
  h5.q-pb-lg I'm Daniel Cortés, a Germany based Colombian film student with a love for documentary, images & stories of all kinds. Currently looking for an internship or a job opportunity.
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
import NaviDesktop from 'components/NaviDesktop'

export default {
  name: 'About',
  components: { NaviDesktop },
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
