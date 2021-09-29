<template>
  <div id="app">      
    <Header/>
    
    <main>
      <Comics/>
    </main>
    
    <Footer/>
  </div>
</template>

<script>
import Header from '@/components/Header.vue';
import Comics from '@/components/Comics.vue';
import Footer from '@/components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Comics,
    Footer
  }
}
</script>

<style lang="scss">
  @import './assets/style/General'; 
</style>
