<template>
  <div id="app">
    <header>
      <Header/>
    </header>
    <main>
      <Comics/>
    </main>
    <footer>
      <Footer/>
    </footer>
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

</style>
