<template>
  <div id="app">      
    <Header/>
    
    <main>
      <Hero/>
      <ComicsFirstSection/>
      <ComicsSecondSection/>
    </main>
    
    <Footer/>
  </div>
</template>

<script>
import Header from '@/components/Header.vue';
import Hero from '@/components/Hero.vue';
import ComicsFirstSection from '@/components/ComicsFirstSection.vue';
import ComicsSecondSection from '@/components/ComicsSecondSection.vue';
import Footer from '@/components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Hero,
    ComicsFirstSection,
    ComicsSecondSection,
    Footer
  }
}
</script>

<style lang="scss">
  @import './assets/style/General'; 
</style>
