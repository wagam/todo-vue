<template>
  <div id="app">
    <Navbar/>
    <Input v-on:add-item="addInputToList"/>
    <TodoList v-bind:items="items"/>

  </div>
</template>

<script>
//import HelloWorld from "./components/HelloWorld.vue";
import Navbar from './components/Navbar.vue';
import Input from './components/Input.vue';
import TodoList from './components/TodoList.vue';

export default {
  name: 'app',
  components: {
    Navbar,
    Input,
    TodoList
  },
  data: function() {
    return {
      items: []
    };
  },
  methods: {
    addInputToList: function(item) {
      this.items.push(item);
      item = '';
    }
  }
};
</script>

<style >
@import '../node_modules/bulma/css/bulma.css';
</style>
