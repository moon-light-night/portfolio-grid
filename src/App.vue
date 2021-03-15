<template>
  <div id="app">
    <a name="home"></a>
    <Arrow></Arrow>
    <Header></Header>
    <About></About>
    <Skills></Skills>
    <Portfolio></Portfolio>
    <Footer></Footer>
  </div>
</template>

<script>
import Arrow from './components/Arrow.vue'
import Header from './components/Header.vue'
import About from './components/About.vue'
import Skills from './components/Skills.vue'
import Portfolio from './components/Portfolio.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Arrow,
    Header,
    About,
    Skills,
    Portfolio,
    Footer,
  },
}
</script>

<style lang="scss"></style>
