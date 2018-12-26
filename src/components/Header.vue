<template>
  <div id="header">
    <h1><router-link to="/">nami634</router-link></h1>
    <ul>
      <li>
        <router-link to="/about">about</router-link>
      </li>
      <li>
        <router-link to="/works">works</router-link>
      </li>
      <li>
        <router-link to="/blog">blog</router-link>
      </li>
    </ul>
  </div>
</template>

<script>
  export default {
    name: 'Header'
  }
</script>

<style lang="scss" scoped>
  #header {
    position: fixed;
    top: 0;
    width: 90vw;
    margin: 0 5vw;
    text-align: right;
    bottom: auto;
    left: auto;
    right: auto;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  ul {
    width: 40vw;
    display: inline-flex;
    justify-content: space-around;
  }

  li {
    list-style-type: none;
    width: 25%;

    a {
      text-decoration: none;
    }
  }
</style>
