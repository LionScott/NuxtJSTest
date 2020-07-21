<template>
  <div class="guide">
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
      <el-menu-item class="none-hover"><input :placeholder="search" />搜索</el-menu-item>
    </el-menu>
  </div>
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
element.style {
  height: 82px;
}

.el-menu {
  border-right-width: 0;
  border: lightblue;
  background-color: #20b2aa;
}

.menu_title {
  flex-direction: row;
}

.el-menu-item {
  line-height: 40px;
  box-sizing: initial;
}

.guide {
  margin: 0;
  padding: 0;
  overflow-x: hidden;
}

.guide ul {
  height: 80px;
  flex: auto;
}

.guide ul li {
  height: 80px;
}

.el-menu--horizontal>.el-menu-item:not(.is-disabled):focus,.el-menu--horizontal>.el-menu-item:not(.is-disabled):hover,.el-menu--horizontal>.el-submenu .el-submenu__title:hover {
    background-color: #20b2aa;
}

.el-menu-item .search:hover {
  background-color: #20b2aa;
}
</style>