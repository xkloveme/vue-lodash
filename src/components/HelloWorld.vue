<template>
  <div class="hello">
    {{list}}
    <p>{{res}}</p>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      list: ['a', 'b', 'c', 'd'],
      res: null
    }
  },
  mounted () {
    this.res = this._.chunk(this.list, 3)
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
