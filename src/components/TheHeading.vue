<template>
  <el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect">
    <el-menu-item index="1">Processing Center</el-menu-item>
    <el-submenu index="2">
      <template slot="title">Workspace</template>
      <el-menu-item index="2-1">item one</el-menu-item>
      <el-menu-item index="2-2">item two</el-menu-item>
      <el-menu-item index="2-3">item three</el-menu-item>
    </el-submenu>
    <el-menu-item index="3"><a href="https://www.ele.me" target="_blank">Orders</a></el-menu-item>
  </el-menu>
</template>

<script>
  export default {
    name: 'the-heading',
    data() {
      return {
        activeIndex: '1',
      };
    },
    methods: {
      handleSelect(key, keyPath) {
        // eslint-disable-next-line
        console.log(key, keyPath);
      },
    },
  };
</script>

<style>
.the-sidebar {
  background-color: #545c64;
  height: 100vh;
}

.the-sidebar .el-menu {
  border: none;
}

.the-sidebar .logo {
  text-align: center;
}

.the-sidebar h1 {
  margin: 0;
  padding: 10px;
  color: #fff
}
</style>
