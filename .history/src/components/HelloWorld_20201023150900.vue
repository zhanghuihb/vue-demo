<template>
  <div class="hello">
    <span v-bind:title="msg">
      鼠标悬停几秒钟查看此处动态绑定的提示信息！
    </span>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: '页面加载于 ' + new Date().toLocaleString()
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
