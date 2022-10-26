<template>
  <TopBg/>
  <div class="listWrap" >
    <ul>
      <li v-for="BolgList in BlogData" :key="BolgList.number">
        <span class="idx">{{BolgList.number}}</span>
          <router-link :to="'/detail/'+BolgList.number">{{ BolgList.title }}</router-link>
         <p class="date">{{ BolgList.date }}</p>
      </li>
    </ul>

  </div>
</template>

<script>
import TopBg from "@/components/TopBg";

export default {
  name: "List",
  components: {TopBg},
  props: {
    BlogData: Array,
  }
}

// :to="{path:'/detail/'+BolgLists.number}"
// `/detail/${BolgLists.number}`
</script>

<style scoped>
*{list-style: none; }
a{text-decoration: none; display:block; font-size:18px; transition: 0.2s all; color:#333;}
.listWrap li:hover{background:red; color:#fff;}
.listWrap li:hover a{ color:#fff;}
.listWrap li{
  padding:10px;
  justify-content: flex-start;
  position: relative;
  width: 100%;
  display:flex;
  border-bottom: 1px solid #ddd;
  align-items: center

}
span{margin-right:20px; }
ul{padding-left:0; box-sizing: border-box;}
.listWrap li h2{}

.date {
  position: absolute;
  right: 20px;
  top:50%;
  transform: translateY(-50%);
}
</style>