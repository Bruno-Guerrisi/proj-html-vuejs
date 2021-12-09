<template>
  <div id="app">

    <header>
      <NavHeader />
    </header>

    <main>
      <MainIntro />
    </main>
    
  </div>
</template>

<script>
import NavHeader from '@/components/NavHeader.vue'
import MainIntro from '@/components/MainIntro.vue'

export default {
  name: 'App',
  components: {
    NavHeader,
    MainIntro,
  }
}
</script>

<style lang="scss">
@import '@/style/global';
@import '@/style/variables';

</style>
