<template>

  <div class="section_main">
    <div class="top_bg">
      <h5>개발자 블로그 </h5>
      <p>Vue 로 만듬</p>
    </div>
  </div>

</template>

<script>
export default {
  name: "TopBg",
  props: {
    BlogData: Array,
  },
}
</script>

<style scoped>
.section_main{}
.top_bg {
  background: #333;
  box-sizing: border-box;
  padding: 25px;
  color: #fff;
}

.top_bg h5 {
  font-size: 24px;
}
.center_class{display:flex;align-items: center;justify-content: center; }

</style>