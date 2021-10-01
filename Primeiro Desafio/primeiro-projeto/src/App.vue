<template>
  <div id="app">
    <!--<img alt="Vue logo" src="./assets/logo.png">-->
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <NovoComponente/>
    <TesteIf/>
    <TesteFor/>
    <TesteEvento/>
    <SitesFavoritos/>
    <DesafioContador/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import NovoComponente from './components/NovoComponente.vue'
import TesteIf from './components/TesteIf.vue'
import TesteFor from './components/TesteFor.vue'
import TesteEvento from './components/TesteEvento.vue'
import SitesFavoritos from './components/SitesFavoritos.vue'
import DesafioContador from './components/DesafioContador.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    NovoComponente,
    TesteIf,
    TesteFor,
    TesteEvento,
    SitesFavoritos,
    DesafioContador,
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
