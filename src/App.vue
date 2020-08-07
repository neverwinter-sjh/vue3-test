<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld :message="state.msg" />
  </div>
</template>

<script>
import { reactive } from 'vue';
import HelloWorld from './components/HelloWorld';

export default {
  name: 'App',  
  components: {
    HelloWorld
  },
  setup() {
    const state = reactive({
      msg: 'Hello!'
    });
    return {
      state
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
