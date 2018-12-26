<template>
  <div id="app">
    <main_header/>
    <router-view/>
  </div>
</template>

<script>
  import main_header from '@/components/Header'
  import 'normalize.css'
  export default {
    components: {
      main_header
    }
  }
</script>

<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }

  a {
    text-decoration: none;
    color: #373737;
  }
</style>
