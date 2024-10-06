<template>
  <select v-model="selectedModel">
    <option value="gpt-3.5">GPT-3.5</option>
    <option value="gpt-4">GPT-4</option>
    <option value="custom">自定义模型</option>
  </select>
</template>

<script setup>
import { ref } from 'vue';

const selectedModel = ref('gpt-3.5');
</script>

<style scoped>
select {
  margin-right: 10px;
  padding: 5px;
}
</style>
