<template>
  <div class="bill">
    <h1>Invoice</h1>
    <h3 class="cafe-name">Helly Chelly Cafe</h3>
    <table class="detail">
      <tbody>
        <tr>
          <td>Table Number:</td>
          <td>
            <input type="text">
          </td>
        </tr>
        <tr>
          <td>Customer Name:</td>
          <td>
            <input type="text">
          </td>
        </tr>
      </tbody>
    </table>
    <div>
      <table class="invoice-detail">
        <thead>
          <tr>
            <td>#</td>
            <td>Particular</td>
            <td>Rate</td>
            <td>Qty</td>
            <td>Amt</td>
          </tr>
        </thead>
      </table>
    </div>

  </div>
</template>

<script>
export default {
  name: 'HcBill',
  data () {
    return {
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.cafe-name {
  margin-top: -10px
}
.detail {
  width: 100%;
  padding: 4px;
}
table.invoice-detail {
  width:100%;
}
table.invoice-detail tr td {
  border: 1px solid black;
}
</style>
