<template>
  <div id="app">
    <Header></Header>
    <About></About>
    <Skills></Skills>
    <Portfolio></Portfolio>
    <Contacts></Contacts>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import About from './components/About.vue'
import Skills from './components/Skills.vue'
import Portfolio from './components/Portfolio.vue'
import Contacts from './components/Contacts.vue'

export default {
  name: 'App',
  components: {
    Header,
    About,
    Skills,
    Portfolio,
    Contacts,
  },
}
</script>

<style lang="scss"></style>
