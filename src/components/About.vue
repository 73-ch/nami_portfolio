<template>
  <div id="about-wrapper" class="wrapper">
    <p>About</p>
    <h1>Kosaku Namikawa</h1>
    <table id="career">
      <tr v-for="event in events" :key="event.title">
        <td>{{event.date}}</td>
        <td>{{event.title}}</td>
      </tr>
    </table>
  </div>
</template>

<script>
  import profile_csv from '@/assets/profile.csv'

  export default {
    name: 'About',
    data() {
      return {
        events: profile_csv
      }
    }
  }
</script>

<style scoped>
  #career {
    text-align: left;
  }
</style>
