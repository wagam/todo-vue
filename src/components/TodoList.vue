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
        <tr>
          <td v-for="item of items" >
            {{item}}
          </td>
          <td><button class="button is-link"><i class="fas fa-trash"></i></button></td>
        </tr>
      </tbody>
    </table>
  </div>
</template>
<script>
export default {
 name: 'TodoList',
 data: function () {
   return {
     items: ['test']
   }
 },
 props: {

 }
}
</script>
<style>

</style>