<template>
  <div id="app">
    <!-- <header>回收站</header> -->
    <!-- <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js + TypeScript App"/> -->
    <!-- <ul>
      <li><a href='/about'>Git基本操作</a></li>
      <li>未完待续。。。</li>
    </ul> -->
    <router-view/>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import HelloWorld from './components/HelloWorld.vue';

@Component({
  components: {
    HelloWorld,
  },
})
export default class App extends Vue {}
</script>

<style lang="less">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  height: 100vh;
  background: black;
}
body {
  margin: 0;
  min-width: 400px;
}
header {
  color: rgb(177, 230, 223);
  min-height: 10vh;
  box-shadow: 0 0 5px #888888;
  font-size: 7vh;
  letter-spacing: 30px;
  font-family: cursive;
}
ul {
  margin: 5vh 0 0 45vw;
  list-style: none;
  li, a {
    text-align: left;
    color: white;
  }
  a:link {
    text-decoration: none;
  }
}
</style>
