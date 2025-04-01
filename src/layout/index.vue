<template>
  <div class="layout">
    <el-container>
      <el-aside width="200px">
        <ul>
          <li>
            <router-link to="/index">后台-主页</router-link>
          </li>
          <li>
            <router-link to="/system/user">后台-系统-用户</router-link>
          </li>
          <li>
            <router-link to="/login">登录</router-link>
          </li>
          <li>
            <router-link to="/signin">注册</router-link>
          </li>
        </ul>
      </el-aside>
      <el-container>
        <el-header>Header</el-header>
        <el-main>
          <router-view></router-view>
        </el-main>
        <el-footer>Footer</el-footer>
      </el-container>
    </el-container>
  </div>
</template>

<script>
export default {
  name: "index"
}
</script>

<style lang="scss" scoped>
.layout {
  width: 100%;
  height: 100%;

  .el-container {
    height: 100%;
  }
}

.el-header, .el-footer {
  background-color: #c6e2ff;
}

.el-aside {
  background-color: #d9ecff;
}

.el-main {
  background-color: #ecf5ff;
}
</style>