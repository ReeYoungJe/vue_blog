<template>
  <Header/>


  <router-view :BlogData="BlogData"/>


</template>

<script>


import Header from "./components/Header";
import BlogData from "./assets/data";

export default {
  name: 'App',
  data() {
    return {
      BlogData: BlogData,
    }
  },
  components: {
    Header: Header,  //Header 컴포넌트
  }
}
</script>

<style>

</style>
