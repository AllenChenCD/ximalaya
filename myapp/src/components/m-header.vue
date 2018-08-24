<template>
 <div class="header">
    <img src="https://s1.xmcdn.com/lib/xmweb/images/logo_f4a8f02.png" alt="" class="logo">
    <div class="header-title">
        Allen
    </div>
 </div>
</template>

<script type="text/ecmascript-6">
export default {
  name: "m-header",
  data() {
    return {};
  },
  components: {}
};
</script>

<style scoped>
.header {
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 20px 0;
}
.logo {
  max-width: 100px;
  margin-right: 20px;
}
.header-title {
  color: #fff;
}
</style>
