<template lang="pug">
div.flex.space-around.q-my-lg.q-ml-lg.container
  router-link.size(to="/") Daniel Cortés
  div
    router-link.q-mr-md(to="/About") About
    a.q-mr-md(href="mailto:someone@yoursite.com") Contact
    //router-link.q-mr-md(to="/") Eng / Esp
</template>

<script>
export default {
  name: 'NaviMain'
}
</script>

<style lang="sass" scoped>
.container
  position: sticky
  height: 3rem
  top: 30px
  width: 50%
  z-index: 1
  // background-color: $dc-green
.size
  width: 28rem
</style>
