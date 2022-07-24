<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import TheHeader from './components/layout/TheHeader.vue'
import TheSidebar from './components/layout/TheSidebar.vue'
</script>

<template>
  <div class="common-layout">
    <TheHeader height="50px" />

    <ElContainer class="ly_pageBody">
      <TheSidebar />

      <ElMain>
        <RouterView />
      </ElMain>
    </ElContainer>
  </div>
</template>

<style lang="scss" scoped>
$pageBodyHeight: calc(100vh - 50px);

.ly_pageBody {
  min-height: $pageBodyHeight;
  height: $pageBodyHeight;
}
</style>
