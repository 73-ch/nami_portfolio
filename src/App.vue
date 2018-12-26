<template>
  <div id="app">
    <router-view/>
    <ul>
      <li><router-link to="/">home</router-link></li>
      <li><router-link to="/about">about</router-link></li>
      <li><router-link to="/works">works</router-link></li>
      <li><router-link to="/blog">blog</router-link></li>
    </ul>
  </div>
</template>

<script>
export default {
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
</style>
