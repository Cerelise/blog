<template>
  <!-- 面包屑导航 -->
  <div class="indexPage">
    <el-breadcrumb separator-class="el-icon-arrow-right">
      <el-breadcrumb-item :to="{ path: '/' }">首页</el-breadcrumb-item>
      <el-breadcrumb-item v-if="category">{{ category }}</el-breadcrumb-item>
      <el-breadcrumb-item>{{ page_name }}</el-breadcrumb-item>
    </el-breadcrumb>
  </div>
</template>

<script>
export default {
  props: ["page_name", "category"],
};
</script>

<style scoped>
.indexPage {
  padding: 10px 10px;
}
</style>
