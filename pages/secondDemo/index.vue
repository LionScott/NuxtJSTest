<template>
  <div>
    <h1>Stars: {{ demoData }}</h1>
    <div>
      <form action>
        <el-input v-model="demoData" pattern="([a-z]|[A-Z]|[0-9])*"></el-input>
        <el-button type="submit" class="el-icon-search"></el-button>
      </form>
    </div>
    <a :href="url">baidu</a>
  </div>
</template>


<script>
export default {
  layout: "demo",
  data() {
    return {
      demoData: "demoData",
      url: "http://www.baidu.com"
    };
  }
};
</script>