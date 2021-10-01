<template>
  <div id="app">      
    <Header/>
    
    <main>
      <Hero :heroUrl="`images/jumbotron.jpg`" :heroAlt="`Hero Image`"/>
      <ComicsFirstSectionSeries/>
      <ComicsSecondSection/>
    </main>
    
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Hero from './components/Hero.vue';
import ComicsFirstSectionSeries from './components/ComicsFirstSectionSeries.vue';
import ComicsSecondSection from './components/ComicsSecondSection.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Hero,
    ComicsFirstSectionSeries,
    ComicsSecondSection,
    Footer
  }
}
</script>

<style lang="scss">
  @import './assets/style/General'; 
</style>
