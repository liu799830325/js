<template>
  <div id="app">
    
    <div fixed class="header">欢迎来到这里</div>
    <Header />
    <router-view/>
    <Bottom />
    <!-- <NavButton /> -->
  </div>
</template>

<script>
import Header from "./components/Header";
import Bottom from "./components/Bottom";
export default {
  name: 'App',
  components: {
    // NavButton,
    // Banner,
    Bottom,
    Header
  },
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
.header{
  position:fixed;
  width: 100%;
  color:red;
  font-size: 30px;
  line-height:50px;
  height: 50px;
  background: blue;
  top:0;
  /* margin-top: -60px; */
}
</style>
