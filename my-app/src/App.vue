<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <Badge caption="Votes"></Badge>
  <Dropdown></Dropdown>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Badge from './components/Badge.vue';
import Dropdown from './components/Dropdown.vue';
// import DropdownItem from './components/DropdownItem.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,
    Badge,
    Dropdown,
    // DropdownItem
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
