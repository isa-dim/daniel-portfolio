<template lang="pug">
NaviDesktop
div
  router-view

</template>

<script>
import { defineComponent } from 'vue'
import NaviDesktop from 'components/NaviDesktop'

export default defineComponent({
  name: 'MainLayout',
  components: { NaviDesktop }
})
</script>
