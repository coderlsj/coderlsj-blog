<template>
<div id="navbar">
  <el-menu
    class="el-menu-demo"
    mode="horizontal"
    default-active="1"
    background-color="#545c64"
    text-color="#fff"
    :router="true"
    active-text-color="#ffd04b">
    <el-input placeholder="请输入内容" class="input-with-select">
      <el-button slot="append" icon="el-icon-search"></el-button>
    </el-input>
    <el-menu-item index="1" route="/home">首页</el-menu-item>
    <el-menu-item index="2" route="/category">目录</el-menu-item>
    <el-menu-item index="3" route="/home">标签</el-menu-item>
    <el-menu-item index="4" route="/home">关于小李</el-menu-item>
  </el-menu>
</div>
</template>

<script>
export default {
  name: 'NavBar'
}
</script>

<style>
#navbar{
  background-color: #545c64;
}
.el-menu-demo{
  display: flex;
  line-height: 61px;
}
</style>