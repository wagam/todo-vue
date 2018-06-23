<template>
<div class="field">
  <label class="label">Name</label>
  <div class="control">
    <input class="input" type="text" placeholder="Add element" v-model="input"/>
  </div>
  <button class="button is-link" v-on:click="$emit('add-item', input)">Add</button>
  <button class="button is-danger" v-on:click="resetInput">Clear</button>
</div>
</template>
<script>
export default {
  name: 'Input',
  data: function() {
    return {
      input: ''
    };
  },
  methods: {
    resetInput() {
      this.input = '';
    }
  }
};
</script>
<style>
</style>