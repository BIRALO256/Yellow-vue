<template>
  
  <Signup></Signup>

</template>

<script>

import Signup from './components/SignupForm.vue'

export default {
  name: 'App',
  components: {
    Signup
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
body{
  margin:0px;
  background:rgb(209, 209, 191);
}
</style>
