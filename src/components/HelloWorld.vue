<template>
  <div class="hello">
    <!-- <span v-bind:title="msg">
      鼠标悬停几秒钟查看此处动态绑定的提示信息！
    </span> -->
    <!-- <p>{{msg}}</p>
    <button v-on:click="reverseMessage">反转消息</button> -->
    <p>{{msg}}</p>
    <input v-model="msg">
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Hello Vue.js'
    }
  },
  methods: {
    reverseMessage: function () {
      this.msg = this.msg.split('').reverse().join('')
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
