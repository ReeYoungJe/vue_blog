<template>
  <Header/>


  <div class="container mt-4">
    <h5>개발자 블로그 </h5>
    <p>Vue 로 만듬</p>
  </div>
  <List :BlogData="BlogData" />
</template>

<script>


import Header from "./components/Header";
import List from "@/components/List";
import BlogData from "./assets/data";
export default {
  name: 'App',
  data(){
    return{
      BlogData : BlogData,
    }
  },
  components : {
    Header,
    List,
  }
}
</script>

<style>

</style>
