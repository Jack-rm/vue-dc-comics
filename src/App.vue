<template>
  <div id="app">
    <Header />
    <Main />
    <Features />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Features from './components/Features.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Features,
    Footer
  }
}
</script>

<style lang="scss">
@import "./style/variables.scss";
@import "./style/general.scss";

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
