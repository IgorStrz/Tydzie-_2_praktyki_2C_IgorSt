<template>
  <div id="app">
    <HelloWorld />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
  },
};
</script>

<style>
body{
  background-color: #A6A6A6;
}
#app {
  font-family: arial;
  font-size: 20px;
  color: #0D0D0D;
  text-align: center;
}
</style>
