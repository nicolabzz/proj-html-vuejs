<template>
  <div id="app">
    <HeaderPage />
    <MainPage />
  </div>
</template>

<script>
import HeaderPage from './components/HeaderPage.vue'
import MainPage from './components/MainPage.vue'

export default {
  name: 'App',
  components: {
    HeaderPage,
    MainPage
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
