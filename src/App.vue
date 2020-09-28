<template>
  <div id="app">
    <nav-bar></nav-bar>
    <router-view></router-view>
    <main-tab-bar></main-tab-bar>
  </div>
</template>

<script>
import NavBar from "@/components/navbar/NavBar.vue"
import MainTabBar from "@/views/maintabbar/MainTabBar.vue"

export default {
  name: "App",
  components: {
    NavBar,
    MainTabBar
  }
}
</script>

<style>

</style>
