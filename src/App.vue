<template>
  <div id="app">

    <header>
      <NavHeader />
    </header>

    <main>
      <MainIntro />

      <Statistics />

      <AboutMe />
    </main>
    
  </div>
</template>

<script>
import NavHeader from '@/components/NavHeader.vue'
import MainIntro from '@/components/MainIntro.vue'
import Statistics from '@/components/Statistics.vue'
import AboutMe from '@/components/AboutMe.vue'

export default {
  name: 'App',
  components: {
    NavHeader,
    MainIntro,
    Statistics,
    AboutMe,
  }
}
</script>

<style lang="scss">
@import '@/style/global';
@import '@/style/variables';

header{
  z-index: 4;
}

</style>
