<template>
  <div v-for="BolgList in BlogData" :key="BolgList">
    <h2>{{BolgList.title}}</h2>
    <p>{{BolgList.content}}</p>
    <p>{{BolgList.date}}</p>
  </div>
</template>

<script>
export default {
  name: "List",
  props:{
    BlogData : Array,
  }
}
</script>

<style scoped>

</style>