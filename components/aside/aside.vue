<template>
  <div>
    <el-row class="tac">
      <el-col :span="12">
        <el-menu
          default-active="2"
          class="el-menu-vertical-demo"
          @open="handleOpen"
          @close="handleClose"
        >
          版本 2.11.X
          <br />序 言
          <el-menu-item index="1">
            <i class="el-icon-menu"></i>
            <span slot="title">介 绍</span>
          </el-menu-item>
          <el-menu-item index="2">
            <i class="el-icon-menu"></i>
            <span slot="title">开源贡献指引</span>
          </el-menu-item>
          <el-menu-item index="3" aria-checked="true">
            <i class="el-icon-menu"></i>
            <span slot="title">版本记录</span>
          </el-menu-item>开始使用
          <el-menu-item index="4">
            <i class="el-icon-menu"></i>
            <span slot="title">安 装</span>
          </el-menu-item>
          <el-menu-item index="5">
            <i class="el-icon-menu"></i>
            <span slot="title">项目目录结构</span>
          </el-menu-item>
          <el-menu-item index="6">
            <i class="el-icon-menu"></i>
            <span slot="title">配 置</span>
          </el-menu-item>
          <el-menu-item index="7">
            <i class="el-icon-menu"></i>
            <span slot="title">路 由</span>
          </el-menu-item>
          <el-menu-item index="8">
            <i class="el-icon-menu"></i>
            <span slot="title">视 图</span>
          </el-menu-item>
          <el-menu-item index="9">
            <i class="el-icon-menu"></i>
            <span slot="title">异步数据</span>
          </el-menu-item>
          <el-menu-item index="10">
            <i class="el-icon-menu"></i>
            <span slot="title">资源文件</span>
          </el-menu-item>
          <el-menu-item index="11">
            <i class="el-icon-menu"></i>
            <span slot="title">插 件</span>
          </el-menu-item>
          <el-menu-item index="12">
            <i class="el-icon-menu"></i>
            <span slot="title">模 块</span>
          </el-menu-item>
          <el-menu-item index="13">
            <i class="el-icon-menu"></i>
            <span slot="title">Vuex 状态树</span>
          </el-menu-item>
          <el-menu-item index="14">
            <i class="el-icon-menu"></i>
            <span slot="title">支持 TypeScript</span>
          </el-menu-item>
        </el-menu>
      </el-col>
    </el-row>
  </div>
</template>

<style scoped>
.el-menu {
  border-right-width: 0;
  border: lightblue;
  background-color: #fcfaf9;
  line-height: 40px;
}

.el-menu-item,
.el-submenu__title {
  height: auto;
}

.el-col-12 {
  width: 100%;
}

.el-row {
  height: 600px;
}
</style>

<script>
export default {
  methods: {
    handleOpen(key, keyPath) {
      console.log(key, keyPath);
    },
    handleClose(key, keyPath) {
      console.log(key, keyPath);
    }
  }
};
</script>