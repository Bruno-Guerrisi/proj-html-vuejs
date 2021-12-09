<template>
  <div id="app">

    <header>
      <NavHeader />
    </header>
    
  </div>
</template>

<script>
/* import 'bootstrap/scss/bootstrap.scss' */
import NavHeader from '@/components/NavHeader.vue'

export default {
  name: 'App',
  components: {
    NavHeader,
  }
}
</script>

<style lang="scss">
@import '@/style/global';
@import '@/style/variables';

</style>
