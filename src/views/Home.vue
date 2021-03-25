<template>
  <div class="home">
    <div class="bill-container">
      <hc-bill></hc-bill>
    </div>
    <div class="menu-container">
      <hc-menu></hc-menu>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'
import HcMenu from '@/components/HcMenu.vue'
import HcBill from '@/components/HcBill.vue'

export default {
  name: 'Home',
  components: {
    HcMenu, HcBill
  }
}
</script>

<style scoped>
.menu-container {
  width: 30vw;
  float: left;
  background: #ff0;
}
.bill-container {
  width: 70vw;
  float: right;
  display: inline-block;
}
.home {
  padding-top: 5px;
  border-top: 1px dashed black;
}
</style>
