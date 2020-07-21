<template>
  <div>
    <h1>Stars: {{ demoData }}</h1>
    <div>
      <form action>
        数字或者大小写字母：<input v-model="demoData" pattern="([a-z]|[A-Z]|[0-9])*" />
        <button type="submit" class="el-icon-search"></button>
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