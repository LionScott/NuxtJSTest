<template>
  <div>
    <h1>Stars: {{ demoData }}</h1>
    <div>
      <input v-model="demoData" />
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