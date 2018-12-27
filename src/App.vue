<template>
  <div id="app">
    <main_header/>
    <main_header style="opacity: 0; position: absolute;"/>
    <router-view/>
  </div>
</template>

<script>
  import 'normalize.css'
  import main_header from '@/components/Header'
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
    color: #2c3e50;
    margin-top: 60px;
    /*display: flex;*/
    /*justify-items: center;*/
    /*align-items: center;*/
  }

  a {
    text-decoration: none;
    color: #373737;
  }
</style>
