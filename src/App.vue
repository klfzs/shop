<template>
  <div id="app">
    <router-view></router-view>
    <MainTarBar></MainTarBar>
  </div>
</template>

<script>
import MainTarBar from 'components/contents/maintarbar/MainTarBar'
export default {
  name: 'app',
  components: {
    MainTarBar
  }
}
</script>

<style>
@import 'assets/css/base.css';
</style>
