<template>
 <div class="nav">
    <router-link tag="div" class="tab-item" to="/Home">
      <span class="tab-link">推荐</span>
    </router-link>
    <router-link tag="div" class="tab-item" to="/Catogry">
      <span class="tab-link">分类</span>
    </router-link>
    <router-link tag="div" class="tab-item" to="/rank">
      <span class="tab-link">排行
      </span>
    </router-link>
    <router-link tag="div" class="tab-item" to="/search">
      <span class="tab-link">搜索</span>
    </router-link>
 </div>
</template>

<script type="text/ecmascript-6">
export default {
  name: "m-nav",
  data() {
    return {};
  },
  components: {}
};
</script>

<style scoped>
.nav{
    display: flex;
    justify-content: space-around;
    margin-bottom: 10px;
}
.nav>div{
    width: 25%;
    text-align: center
}
.nav>div span{
    color: #ffffff
}
.router-link-active .tab-link{
    color: crimson;
    border-bottom: 2px solid crimson;
}

</style>
