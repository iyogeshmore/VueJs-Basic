<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <!-- <HelloWorld msg="Hello Vue 3.0 + Vite" /> -->
  <Home/>
  <About/>
  <Addition/>
</template>

<script>

import Home from './components/Home.vue'
import About from './components/About.vue'
import Addition from './components/Addition.vue'

export default {
  name: 'App',
  components: {
    Home,
        About,
        Addition
  }
}
</script>
