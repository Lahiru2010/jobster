<template>
  <div id="app">
    <home></home>
  </div>
</template>

<script>
import Home from './components/Home.vue'
export default {
  name: 'app',
  components: {
    Home
  }
}
</script>

<style lang="scss">  
@import 'src/scss/custom.scss';
 @import '~bootstrap/scss/bootstrap.scss';
 @import '~bootstrap-vue/src/index.scss'; 
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  background-color: #f2f4f8;
  color: #2c3e50;
}
</style>
