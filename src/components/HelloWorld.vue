<template>
  <div>
    <h1>Hello from Jacqueline Taylor & Friends</h1>
  </div>

  <div>{{sourceData}}</div>
</template>

<script>
import sourceData from '@/data.json'
console.log(sourceData)
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
    return {
      threads: sourceData.threads
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
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
