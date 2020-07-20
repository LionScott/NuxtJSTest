
<template>
  <el-container>
    <el-header>
      <Menu class="demo_menu"></Menu>
    </el-header>
    <el-container>
      <el-aside class="demo_aside">
        <Aside></Aside>
      </el-aside>
      <el-main>
        <div class="demo_view">
          <nuxt />
        </div>
      </el-main>
    </el-container>
  </el-container>
</template>

<script>
import Menu from "@/components/header/Menu";
import Aside from "@/components/aside/aside";
export default {
  components: Menu,
  components: Aside
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  overflow-x: hidden;
}
html {
  /* font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif; */
  font-family: "游ゴシック体", YuGothic, "游ゴシック Medium", "Yu Gothic Medium",
    "游ゴシック", "Yu Gothic", "メイリオ", sans-serif;
  color: #606266;
  min-width: 1400px;
}

.el-header {
  margin: 0;
  padding: 0;
  overflow-x: hidden;
  height: 120px;
}

.el-menu--horizontal > .el-menu-item {
  color: aliceblue;
}

.demo_header {
  flex-direction: row;
}

.demo_title {
  background: beige;
}

.demo_aside {
  background-color: rgb(252, 239, 216);
  width: 100px;
  height: 600px;
}

.demo_containt {
  flex-direction: column;
}

.demo_view {
  width: 100%;
  flex-direction: row;
}
</style>
