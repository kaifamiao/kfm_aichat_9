<template>
  <select v-model="selectedOption">
    <option value="1">选项1</option>
    <option value="2">选项2</option>
    <option value="3">选项3</option>
  </select>
</template>

<script setup>
import { ref } from 'vue';

const selectedOption = ref('1');
</script>

<style scoped>
select {
  width: 100px;
  padding: 5px;
}
</style>
