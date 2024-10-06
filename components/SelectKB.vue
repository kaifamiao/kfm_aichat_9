<template>
  <select v-model="selectedKB">
    <option value="none">无知识库</option>
    <option value="kb1">知识库1</option>
    <option value="kb2">知识库2</option>
  </select>
</template>

<script setup>
import { ref } from 'vue';

const selectedKB = ref('none');
</script>

<style scoped>
select {
  padding: 5px;
}
</style>
