<template>
  <div>
    <div>{{v}}</div>

    <div>{{titleShow}}</div>
  </div>
</template>

<script>
import axios from "axios";
export default {
  layout: "demo",
  data() {
    return {
      titleShow: "1111",
      v: undefined
    };
  },
  created() {
    axios.get(process.env.APIROOT + "index").then(res => {
      this.v = res.data.v;
    });
  }
};
</script>

<style scoped>

</style>