<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <TheHeader msg="Hello, Vue Js. This is my component" v-show="showHeader"/>
  <ComponentVIFELSE/>
  <ComponentFor/>
  <RandomImagem/>
</template>

<script>
import TheHeader from './components/TheHeader.vue'
import ComponentFor from './components/ComponentFor.vue'
import ComponentVIFELSE from './components/ComponentVIFELSE.vue'
import RandomImagem from './components/RandomImagem.vue'

export default {
  name: 'App',
  components: {
    TheHeader,
    ComponentFor,
    ComponentVIFELSE,
    RandomImagem
  },
  data () {
    return {

    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
