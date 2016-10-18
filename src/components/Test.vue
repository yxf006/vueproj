
<template>
<div>
  <hr>
  <h5>{{ msg }}</h5>


  <el-row type="flex" class="tac" :gutter="20">

    <el-col :span="4">
      <div class="grid-content bg-purple">
        <el-menu default-active="2" class="el-menu-vertical-demo" @open="handleopen" @close="handleclose">
          <el-submenu index="1">
            <template slot="title"><i class="el-icon-message"></i>导航一</template>
        <el-menu-item-group title="分组一">
          <el-menu-item index="1-1">选项1</el-menu-item>
          <el-menu-item index="1-2">选项2</el-menu-item>
        </el-menu-item-group>
        <el-menu-item-group title="分组2">
          <el-menu-item index="1-3">选项3</el-menu-item>
        </el-menu-item-group>
      </el-submenu>
      <el-menu-item index="2"><i class="el-icon-menu"></i>导航二</el-menu-item>
      <el-menu-item index="3"><i class="el-icon-setting"></i>导航三</el-menu-item>
    </el-menu>
  </div>
  </el-col>
<el-col :span="20">
  <div class="grid-content bg-purple">
  <el-tabs>
    <el-tab-pane label="用户管理"></el-tab-pane>
    <el-tab-pane label="配置管理"></el-tab-pane>
    <el-tab-pane label="角色管理"></el-tab-pane>
    <el-tab-pane label="用户角色管理"></el-tab-pane>
  </el-tabs>
</div>
</el-col>
</div>
</template>

<script>
export default {
  name: 'test',
  data () {
    return {
      activeName:'first',
      msg: 'test components for Test'
    }
  }
}
</script>
