<template>
  <el-menu
    :default-active="activeIndex2"
    class="el-menu-demo"
    mode="horizontal"
    router
    @select="handleSelect"
  >
    <el-menu-item margin="0px 10px 0px 5px">NuxtJS</el-menu-item>
    <el-menu-item index="/">学习指南</el-menu-item>
    <el-menu-item index="/firstDemo">API</el-menu-item>
    <el-menu-item index="/secondDemo">案例</el-menu-item>
    <el-menu-item index="/thirdDemo">常见问题</el-menu-item>
    <el-menu-item index="/forthDemo">BLOG</el-menu-item>
    <el-menu-item index="/fifthDemo">英文官网</el-menu-item>
    <el-menu-item class="search">
      <input :placeholder="search" />搜索
    </el-menu-item>
  </el-menu>
</template>
<script>
export default {
  data() {
    return {
      activeIndex2: "1",
      search: "输入框"
    };
  },
  methods: {
    handleSelect(key, keyPath) {
      console.log(key, keyPath);
    }
  }
};
</script>

<style >
.el-menu {
  border-right-width: 0;
  border: lightblue;
  background-color: #20b2aa;
}

.menu_title {
  flex-direction: row;
}

.el-menu-item {
  line-height: 90px;
  box-sizing: initial;
}

.el-menu-item .search:hover {
  background-color: #20b2aa;
}
</style>