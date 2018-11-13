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
</div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      value1: 50,
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
