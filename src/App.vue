<template>
  <div id="app">
    <el-container>
      <el-aside>
        <the-sidebar/>
      </el-aside>
      <el-container>
        <el-header class="header">
          <the-heading/>
        </el-header>
        <el-main>
          <router-view/>
        </el-main>
        <el-footer>
          <the-footer/>
        </el-footer>
      </el-container>
    </el-container>
  </div>
</template>

<script>
import TheHeading from './components/TheHeading';
import TheFooter from './components/TheFooter';
import TheSidebar from './components/TheSidebar';

export default {
  name: 'app',
  components: { TheHeading, TheFooter, TheSidebar },
};
</script>

<style>
body {
  margin: 0;
  background: #f2f3f8; 
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

.header {
  background: #fff;
}
</style>
