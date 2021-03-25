<template>
  <div class="menu">
    <h1>Menu</h1>
    <table class="table table-bordered">
      <thead>
        <tr>
          <th class="text-left">Name</th>
          <th class="text-right">Price</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="item in menuItems" v-bind:key="item.name">
          <td class="text-left" @click="addItem(item)">{{ item.name }}</td>
          <td class="text-right">{{ item.price }}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
export default {
  name: 'HcMenu',
  data: function () {
    return {
      menuItems: [
        {
          name: 'Margerita Pizza',
          price: 89
        },
        {
          name: 'Italian Pizza',
          price: 110
        },
        {
          name: 'Pasta',
          price: 99
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
