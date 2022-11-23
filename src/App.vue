<template>
  <div id="app">
    <!-- <NavBar></NavBar> -->
    <HomePage/>
  </div>
</template>



<script>
import HomePage from './views/HomePage.vue';
// import NavBar from './widgets/NavBar.vue';

export default {
  name: 'App',
  components: {
    HomePage,
    // NavBar
}
}
</script>

<style>
/* #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
} */
</style>