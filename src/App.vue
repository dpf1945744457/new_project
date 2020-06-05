<template>
  <div id="app">
    <!-- 显示主页 -->
    <el-container class="app-container">
      <!-- 左侧导航菜单 -->
      <el-aside width="200px">Aside</el-aside>

      <el-container>
        <!-- 顶部区域 -->
        <el-header class="app-header">Header</el-header>

        <!-- 内容主体区域 -->
        <el-main class="app-main">Main</el-main>

        <!-- 底部区域-->
        <el-footer class="app-footer">Footer</el-footer>
      </el-container>
    </el-container>
  </div>
</template>

<script>
export default {
  name: "App"
};
</script>

<style >
html,
body {
  padding: 0;
  margin: 0;
  width: 100%;
  height: 100%;
  background: rgba(247, 248, 250, 1);
}
#app {
  height: 100%;

}
.app-container {
  height: 100%;
}
.app-header {
  padding-left: 0;
  padding-right: 0;
}
.app-main {
  padding-bottom: 0;
  padding-right: 0;
}
.app-footer {
  padding-bottom: 0;
  padding-right: 0;
}
</style>
