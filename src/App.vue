<template>
  <div id="app" class="m-0 p-0 bg-dark">
    <top-bar></top-bar>
    <side-bar></side-bar>
    <router-view/>
  </div>
</template>

<script>
import SideBar from './components/SideBar.vue'
import TopBar from './components/TopBar.vue'

export default {
  name: 'App',
  components: {
    TopBar,
    'side-bar': SideBar
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
</style>
