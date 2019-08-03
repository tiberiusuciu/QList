<template>
  <div id="app">
    <AddBar />
    <h2>{{$store.state.inputText}}</h2>
  </div>
</template>

<script>
import AddBar from './components/AddBar.vue'

export default {
  name: 'app',
  components: {
    AddBar
  }
}
</script>

<style>
body, h1, h2, h3, h4, h5, h6, html, head, p, div {
  margin: 0px;
  padding: 0px;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: ghostwhite;
  height: 100vh;
  width: 100%;
}
</style>
