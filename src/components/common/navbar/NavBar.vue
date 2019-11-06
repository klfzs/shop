<template>
  <div class="nav-bar">
     <div class="left"> <slot name="left"></slot> </div>
     <div class="centen">  <slot name="centen"></slot>  </div>
     <div class="right"> <slot name="right"></slot> </div>
  </div>
</template>

<script>
export default {
    name:'NavBar'
}
</script>

<style>
.nav-bar
{
    display: flex;
    text-align: center;
    line-height: 44px;
    color: white;
    background-color: pink;
    box-shadow: 0px 1px 1px rgba(100,100,100, .1)
}
.left{
    width: 45px;
}
.centen{
    flex: 1;
}
.right{
    width: 45px;
    background-color:pink; 
}
</style>