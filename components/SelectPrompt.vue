<template>
  <select v-model="selectedPrompt">
    <option value="default">默认提示词</option>
    <option value="prompt1">提示词1</option>
    <option value="prompt2">提示词2</option>
  </select>
</template>

<script setup>
import { ref } from 'vue';

const selectedPrompt = ref('default');
</script>

<style scoped>
select {
  margin-right: 10px;
  padding: 5px;
}
</style>
