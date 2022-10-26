<template>

  <div>
    <TopBg/>
    <div class="">

    </div>

    <p @click="$router.go(-1)">◀</p>

    <div class="no">
      <p>{{ $route.params.id }}번 게시물</p>
    </div>
    <div class="title">
      <h2>{{ BlogData[$route.params.id].title }}</h2>
    </div>
    <div class="content">
      <div>{{ BlogData[$route.params.id].content }}</div>
    </div>

  </div>

</template>

<script>
import TopBg from "@/components/TopBg";

export default {
  name: "Detail",
  components: {TopBg},
  props: {
    BlogData: Array,
  },
}
</script>

<style scoped>
.no{text-align: center}
.title{text-align: center; padding-bottom: 30px; margin-bottom:40px; border-bottom: 1px solid #ddd;}
.content{ text-align: center;}
</style>