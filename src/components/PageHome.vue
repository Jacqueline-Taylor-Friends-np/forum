<template>
  <div><h2>Jacqueline's Forum</h2></div> <!-- TODO: google forum -->
  <div v-for="thread in threads" :key="thread.id">
      <h2>{{thread.title}}</h2>
  </div>


</template>

<script>
// import data
import sourceData from '@/data.json'
export default {
  data() {
    return {
      threads: sourceData.threads
    }
  }
}
</script>

<style scoped>

</style>
