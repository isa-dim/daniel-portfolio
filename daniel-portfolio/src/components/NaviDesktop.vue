<template lang="pug">
div.flex.justify-between.q-ma-lg
  router-link.q-mr-md(to="/") Daniel Cortés
  div
    router-link.q-mr-md(to="/About") About
    a.q-mr-md(href="mailto:someone@yoursite.com") Contact
    router-link.q-mr-md(to="/") Eng / Esp
</template>

<script>
export default {
  name: 'NaviDesktop'
}
</script>

<style lang="sass" scoped>
</style>
