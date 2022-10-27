<template>
  <div class="direction">
    <ul>
      <li><span @click="$router.go(-1)">이전</span></li>
      <li><router-link to="/">Home</router-link></li>
      <li><span @click="$router.go(+1)">다음</span></li>
    </ul>
  </div>

</template>

<script>

export default {
  name: "Direction",
}
</script>

<style scoped>

</style>