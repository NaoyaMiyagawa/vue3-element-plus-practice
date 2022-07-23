<script setup lang="ts">
import { ref } from 'vue';
const selected = ref();
</script>

<template>
  <div class="about">
    <h1>This is an about page</h1>
    <div class="bg-light-200">
      <ElButton>aaa</ElButton>

      <div>
        {{ selected }}
        <ElSelect v-model="selected">
          <ElOption disabled value="">Please select one</ElOption>
          <ElOption value="1">1</ElOption>
          <ElOption value="2">2</ElOption>
          <ElOption value="3">3</ElOption>
        </ElSelect>
      </div>
    </div>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
