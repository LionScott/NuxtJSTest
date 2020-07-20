<template>
  <div>
    <el-table :data="guide">
      <el-table-column prop="id" label="ID" width="180"></el-table-column>
      <el-table-column prop="title" label="title" width="180"></el-table-column>
      <el-table-column prop="content" label="content"></el-table-column>
    </el-table>

    <div class="block">
      <span class="demonstration">完整功能</span>
      <el-pagination
        @size-change="handleSizeChange"
        @current-change="handleCurrentChange"
        :current-page="currentPage4"
        :page-sizes="[100, 200, 300, 400]"
        :page-size="100"
        layout="total, sizes, prev, pager, next, jumper"
        :total="400"
      ></el-pagination>
    </div>
  </div>
</template>


<script>
export default {
  layout: "demo",
  methods: {
    handleSizeChange(val) {
      console.log(`每页 ${val} 条`);
    },
    handleCurrentChange(val) {
      console.log(`当前页: ${val}`);
    }
  },
  data() {
    return {
      currentPage1: 5,
      currentPage2: 5,
      currentPage3: 5,
      currentPage4: 4,
      guide: [
          { id: 1, title: "安 装", content: "content txt for install" },
          { id: 2, title: "项目目录结构", content: "" },
          { id: 3, title: "配 置", content: "" },
          { id: 4, title: "路 由", content: "" },
          { id: 5, title: "视 图", content: "" },
          { id: 6, title: "异步数据", content: "" }
        ]
    };
  }
};
</script>