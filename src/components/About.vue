<template>
  <div id="about-wrapper" class="wrapper">
    <h1 class="component-title">- About -</h1>
    <div id="name">
      <h3 class="section-title">Name / 名前</h3>
      <div id="name-box">
        <img src="../assets/image/test.png" alt="nami634_icon">
        <div>
          <h2>Kosaku Namikawa</h2>
          <h2>浪川 洪作</h2>
        </div>
      </div>
    </div>
    <div id="skill">
      <h3 class="section-title">Skills / スキル</h3>
      <p>WebGL, Ruby on Rails, Node.js, GLSL, openFrameworks, MaxMSP...</p>
    </div>
    <div id="career">
      <h3 class="section-title">Career / 経歴</h3>
      <table>
        <tr v-for="event in events" :key="event.title">
          <td>{{event.date}}</td>
          <td>{{event.title}}</td>
        </tr>
      </table>
    </div>
  </div>
</template>

<script>
  import '@/assets/css/common.scss'
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

<style lang="scss" scoped>
  @import '../assets/css/media_queries';

  .section-title {
    font-size: 2vw;
    margin: 1vh 0;
  }

  %section {
    margin: 5vh 0;
  }

  #skill {
    @extend %section;

    p {
      font-size: 1vw;
    }
  }

  #career {
    @extend %section;

    table {
      font-size: 1vw;
    }
  }

  #name {
    @extend %section;

    #name-box {
      display: flex;
      justify-content: space-between;

      div {
        display: inline-flex;
        flex-direction: column;
        justify-content: center;

        h2 {
          font-size: 4.5vw;
          margin-top: 1.5vh;
          display: inline-block;
        }

        h2:lang(ja) {
          font-size: 7.5vw;
        }
      }

      img {
        width: 30vw;
        height: 30vw;

        @include mq(sm) {
          width: 60vw;
          height: 60vw;
        }
      }
    }
  }
</style>
