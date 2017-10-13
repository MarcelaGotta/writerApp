<template>
  <div class="the-sidebar">
    <div class="logo">
      <h1>writerApp</h1>
      <i class="fa el-icon-fa-address-book" aria-hidden="true"></i>
    </div>
    <el-menu
      default-active="2"
      class="el-menu-vertical-demo"
      @open="handleOpen"
      @close="handleClose"
      background-color="#545c64"
      text-color="#fff"
      active-text-color="#ffd04b">
      <el-menu-item index="0-1">Tablero</el-menu-item>
      <el-submenu index="characters">
        <template slot="title">
          <i class="el-icon-message"></i>
          <span>Personajes</span>
        </template>
        <el-menu-item index="c-first">Principales</el-menu-item>
        <el-menu-item index="c-sec">Secundarios</el-menu-item>
      </el-submenu>
      <el-menu-item index="places">Lugares</el-menu-item>
      <el-menu-item index="2">
        <i class="el-icon-menu"></i>
        <span>Navigator Two</span>
      </el-menu-item>
      <el-menu-item index="3">
        <i class="el-icon-setting"></i>
        <span>Navigator Three</span>
      </el-menu-item>
    </el-menu>
  </div>
</template>

<script>
export default {
  name: 'theSidebar',
  methods: {
    handleOpen(key, keyPath) {
      // eslint-disable-next-line
      console.log(key, keyPath);
    },
    handleClose(key, keyPath) {
      // eslint-disable-next-line
      console.log(key, keyPath);
    },
  },
};
</script>

<style>

</style>
