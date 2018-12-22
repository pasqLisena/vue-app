<template>
<div id="app">
  <img alt="Vue logo" src="./assets/logo.png">
  <!-- use hyphenated names! --> <child :my-message="msg"></child>
</div>
</template>

<script>
import Child from './components/Child.vue';

export default {
  name: 'app',
  components: {
    Child
  },
  // https://vuejs.org/2016/02/06/common-gotchas/#Why-does-data-need-to-be-a-function
  data: () => ({
    msg: 'Hello Vue.js!'
  }),
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
