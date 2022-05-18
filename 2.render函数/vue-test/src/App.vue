<template>
  <div id="app">
    <span>render函数</span>
    <RenderTest tag="ul" />
  </div>
</template>

<script>
import RenderTest from './components/RenderTest.vue'

export default {
  name: 'App',
  components: {
    RenderTest
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
