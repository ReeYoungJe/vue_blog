<template>
  <Header/>


  <div class="container mt-4">
    <h5>개발자 블로그 </h5>
    <p>Vue 로 만듬</p>
  </div>

  <div>
    <router-view :BlogData="BlogData" />
  </div>

</template>

<script>


import Header from "./components/Header";
import BlogData from "./assets/data";

export default {
  name: 'App',
  data(){
    return{
      BlogData : BlogData,
    }
  },
  components : {
    Header : Header,  //Header 컴포넌트
  }
}
</script>

<style>

</style>
