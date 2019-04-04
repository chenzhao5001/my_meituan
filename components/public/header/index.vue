<template>
  <el-row :gutter="0" class="m-header">
    <el-col :span="2">11</el-col>
    <el-col :span="2">22</el-col>
    <el-col :span="2">333</el-col>
  </el-row>
</template>

<script>
  // import geo from "./geo"
  export default {
    name: "index",
    components:{
      // geo
    }
  }
</script>

<style lang="scss" scoped>
  .test {
    background: red;
  }
  /*@import '@/asserts/css/public/header/header.scss';*/
  @import "@/assets/css/public/header.scss";
</style>
