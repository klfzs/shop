<template>
  <div id="home">
    <NavBar>
      <template v-slot:centen>
        <div>购物街</div>
      </template>
    </NavBar>
    <HomeSwiper :cbanners='banners'></HomeSwiper>
  </div>
</template>

<script>
import NavBar from 'components/common/navbar/NavBar'
import HomeSwiper from "./childComps/HomeSwiper"
import { getHomeMultidata } from "network/home"

export default {
   name:'home',
  data(){
    return{
      banners:[],
      recommends:[]
    }
  }, 
  components:{
    NavBar,
    HomeSwiper
  },
  created(){
    getHomeMultidata().then(res=>{
     this.banners=res.data.data.banner.list;
     console.log(this.banners);
     this.recommends=res.data.data.recommend.list;

    })
  }
}
</script>

<style scoped>



</style>
