<template>
  <div class="hello">
    <input type="number" v-model.number="value" v-focus="red">
    <div>{{value | toFixed | fillZero}}</div>
    <div>{{0.1 | toFixed}}</div>
  </div>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      value: 1,
      num: 10.232323
    }
  },
  // computed: {
  //   numFixed () {
  //     return  this.value.toFixed(2)
  //   }
  // }
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
