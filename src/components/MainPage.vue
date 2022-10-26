<template>

  <div class="section_main">
    <TopBg></TopBg>
    <div class="center_class">
      메인페이지 입니다

    </div>
  </div>

</template>

<script>
import TopBg from "@/components/TopBg";
export default {
  name: "MainPage",
  components: {TopBg},
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