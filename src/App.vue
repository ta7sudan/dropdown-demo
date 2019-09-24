<template>
  <div id="app">
    <header>
      <el-dropdown>
        <div class="user-dropdown">dropdown</div>
        <el-dropdown-menu slot="dropdown">
          <el-dropdown-item class="fix-width">测试内容1</el-dropdown-item>
          <el-dropdown-item class="fix-width">测试内容2</el-dropdown-item>
          <el-dropdown-item class="fix-width">测试内容3</el-dropdown-item>
        </el-dropdown-menu>
      </el-dropdown>
    </header>
  </div>
</template>

<script>
import { Dropdown, DropdownMenu, DropdownItem } from 'element-ui'

const ElDropdown = Dropdown,
  ElDropdownMenu = DropdownMenu,
  ElDropdownItem = DropdownItem;

export default {
  name: 'app',
  components: {
    ElDropdown,
    ElDropdownMenu,
    ElDropdownItem
  }
}
</script>

<style>
header {
  text-align: right;
  padding: 10px;
  border: 1px solid #000;
  min-width: 800px;
}

.user-dropdown {
  border: 1px solid #000;
  padding: 10px 20px;
  display: inline-block;
}

.fix-width {
  min-width: max-content;
}
</style>
