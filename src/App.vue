<template>
  <div id="app">
    <Navbar/>
    <Input/>
    <TodoList item='test'/>
  </div>
</template>

<script>
//import HelloWorld from "./components/HelloWorld.vue";
import Navbar from "./components/Navbar.vue";
import Input from "./components/Input.vue";
import TodoList from "./components/TodoList.vue";

export default {
  name: 'app',
  components: {
    Navbar,
    Input,
    TodoList
  }
};
</script>

<style >
@import '../node_modules/bulma/css/bulma.css';

</style>
