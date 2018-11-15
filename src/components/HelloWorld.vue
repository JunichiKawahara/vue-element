<template>
<div>
  <div>
    <p>
      使いたい部品は、<a target="_blank" href="http://element.eleme.io/#/en-US/component/layout">
      公式のサイト</a>で確認できる。
    </p>
  </div>
  <div class="block">
    <span class="demonstration">スライダー</span>
    <el-slider v-model="value1"></el-slider>
  </div>
  <div>{{ value1 }}</div>

  <div class="block">
    <span class="demonstration">日付ピッカー</span>
    <el-date-picker
      v-model="valueDate"
      type="date"
      placeholder="日付を選んでください">
    </el-date-picker>
  </div>

  <div class="block" style="background-color: #ffcc66;">
    <span class="demonstration">Table</span>
    <el-table
      v-bind:data="tableData3"
      height="100%"
      style="width: 100%;">
      <el-table-column
        prop="date"
        label="Date"
        width="180">
      </el-table-column>
      <el-table-column
        prop="name"
        label="Name"
        width="180">
      </el-table-column>
      <el-table-column
        prop="address"
        label="Address">
      </el-table-column>
    </el-table>
  </div>

</div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      value1: 50,
      valueDate: '',
      tableData3: [{
          date: '2016-05-03',
          name: 'Tom',
          address: 'No. 189, Grove St, Los Angeles'
        }, {
          date: '2016-05-02',
          name: 'Tom',
          address: 'No. 189, Grove St, Los Angeles'
        }, {
          date: '2016-05-04',
          name: 'Tom',
          address: 'No. 189, Grove St, Los Angeles'
        }, {
          date: '2016-05-01',
          name: 'Tom',
          address: 'No. 189, Grove St, Los Angeles'
        }, {
          date: '2016-05-08',
          name: 'Tom',
          address: 'No. 189, Grove St, Los Angeles'
        }, {
          date: '2016-05-06',
          name: 'Tom',
          address: 'No. 189, Grove St, Los Angeles'
        }, {
          date: '2016-05-07',
          name: 'Tom',
          address: 'No. 189, Grove St, Los Angeles'
      }],
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
