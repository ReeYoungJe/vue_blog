<template>
  <Header/>


  <router-view :BlogData="BlogData"/>

  <direction/>

</template>

<script>


import Header from "./components/Header";
import BlogData from "./assets/data";
import Direction from "@/components/Direction";


export default {
  name: 'App',
  data() {
    return {
      BlogData: BlogData,
    }
  },
  components: {
    Header: Header,  //Header 컴포넌트
    Direction: Direction,
  }
}
</script>

<style>
html{background:#333; display: flex;justify-content: center;}
body{width:720px;margin: 0 auto;border:1px solid #ddd; height:100vh;  position: relative}
*{list-style: none; }
a{text-decoration: none; display:block; font-size:18px; transition: 0.2s all; color:#333;}
.direction{position: absolute; bottom: 0; left: 0; width:100%;}
.direction ul{padding-left: 0 !important; display: flex;align-items: center ;justify-content: space-around}


</style>
