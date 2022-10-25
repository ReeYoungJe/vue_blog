<template>

<div>
  <h2>{{BlogData[$route.params.id].title}}</h2>
</div>

</template>

<script>
export default {
  name: "Detail",
  props:{
    BlogData : Array,
  }
}
</script>

<style scoped>

</style>