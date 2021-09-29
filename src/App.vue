<template>
  <div id="app">      
    <Header/>
    
    <main>
      <ComicsFirstSection/>
      <ComicsSecondSection/>
    </main>
    
    <Footer/>
  </div>
</template>

<script>
import Header from '@/components/Header.vue';
import ComicsFirstSection from '@/components/ComicsFirstSection.vue';
import ComicsSecondSection from '@/components/ComicsSecondSection.vue';
import Footer from '@/components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    ComicsFirstSection,
    ComicsSecondSection,
    Footer
  }
}
</script>

<style lang="scss">
  @import './assets/style/General'; 
</style>
