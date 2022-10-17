<template>
  <div v-for="BlogData">
    <h2>{{BlogData[0].title}}</h2>
    <p>{{BlogData[0].date}}</p>
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