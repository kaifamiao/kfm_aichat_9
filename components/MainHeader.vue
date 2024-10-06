<template>
  <div class="main-header">
    <button @click="$emit('toggleSidebar')">☰</button>
    <SelectModel />
    <SelectPrompt />
    <SelectKB />
  </div>
</template>

<script setup>
import SelectModel from './SelectModel.vue';
import SelectPrompt from './SelectPrompt.vue';
import SelectKB from './SelectKB.vue';
</script>

<style scoped>
.main-header {
  display: flex;
  align-items: center;
  padding: 10px;
  background-color: #eaeaea;
}
.main-header button {
  margin-right: 15px;
  font-size: 24px;
}
</style>
