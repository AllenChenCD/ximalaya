<template>
  <div id="app">
          <MHeader></MHeader >
         <Nav></Nav> 
    <router-view/>
  </div>
</template>

<script>
import MHeader from "components/m-header";
import Nav from "components/m-nav";
export default {
  name: 'App',
  components:{
    MHeader,Nav
  }
}
</script>

<style>
@import 'assets/index.css';
</style>
