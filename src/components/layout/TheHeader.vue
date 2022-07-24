<script setup lang="ts">
//
const loginUser = $ref({ name: 'Tom' })
</script>

<template>
  <ElHeader class="ly_header">
    <div class="toolbar">
      <ElDropdown>
        <ElIcon style="margin-right: 8px; margin-top: 1px"><setting /></ElIcon>

        <template #dropdown>
          <ElDropdownMenu>
            <ElDropdownItem>View</ElDropdownItem>
            <ElDropdownItem>Add</ElDropdownItem>
            <ElDropdownItem>Delete</ElDropdownItem>
          </ElDropdownMenu>
        </template>
      </ElDropdown>

      <span>{{ loginUser.name }}</span>
    </div>
  </ElHeader>
</template>

<style lang="scss" scoped>
.ly_header {
  position: relative;
  background-color: var(--el-color-primary-light-7);
  color: var(--el-text-color-primary);
  text-align: right;
  font-size: 12px;

  .toolbar {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    height: 100%;
    right: 20px;
  }
}
</style>
