<template>
  <div>
    <table class="table">
      <thead>
        <tr>
          <th>Item</th>
          <th>Supprimer</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="(item, index) of items" v-bind:key="index">
          <td >
            {{item}}
          </td>
          <td><button class="button is-link" v-on:click="deleteItemFromList(item)">-</button></td>
        </tr>
      </tbody>
    </table>
  </div>
</template>
<script>
export default {
  props: {
    items: Array
  },
  methods: {
    deleteItemFromList(item) {
      this.items = this.items.filter(i => i !== item);
    }
  }
};
</script>
<style>
</style>