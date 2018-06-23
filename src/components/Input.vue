<template>
<div class="field">
  <label class="label">Name</label>
  <div class="control">
    <input class="input" type="text" placeholder="Add element" v-model="input"/>
  </div>
  <button class="button is-link" v-on:click="$emit('item', input)">Add {{count}}</button>
</div>
</template>
<script>
export default {
  name: 'Input',
  data: function() {
    return {
      count: 0,
      input: ''
    };
  },
  methods: {

  }
};
</script>
<style>
</style>