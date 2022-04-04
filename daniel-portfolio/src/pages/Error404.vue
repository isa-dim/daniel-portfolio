<template lang="pug">
div.row
  div.col-md-6.col-12.left
    div.left-item.flex.column.caudex
      p.q-mt-lg Daniel Cortés
      h3.titulo Film student with a love for images & stories
      div.q-mb-lg.circle-filled
  div.col-md-6.col-12.right
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
        :src="bw"
        fit="cover"
        style="height: 350px; max-width: 20rem")
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'Error404'
})
</script>

<style lang="sass">
.left
  border: 1px solid red
.right
  border: 1px solid blue
</style>
