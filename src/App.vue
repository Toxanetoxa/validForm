<template>
  <div id="app">
    <h1>Hello</h1>
    <t-form/>
  </div>
</template>

<script>

import TForm from "@/components/global/tForm";
export default {
  name: 'App',
  components: {
    TForm
  }
}
</script>

<style>
#app {
  font-family: 'IBM Plex Sans', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
