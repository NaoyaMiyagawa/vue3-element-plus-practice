<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import TheHeader from './components/layout/TheHeader.vue'
</script>

<template>
  <div class="common-layout">
    <TheHeader />

    <ElContainer>
      <ElAside width="200px">Aside</ElAside>
      <ElMain>
        <RouterView />
      </ElMain>
    </ElContainer>
  </div>
</template>

<style lang="scss" scoped>
//
</style>
