<template>
  <div id="home">
    <NavBar>
      <template v-slot:centen>
        <div>购物街</div>
      </template>
    </NavBar>
  </div>
</template>

<script>
import NavBar from 'components/common/navbar/NavBar'


export default {
  name:'home',
  components:{
    NavBar
  }
}
</script>

<style scoped>



</style>
