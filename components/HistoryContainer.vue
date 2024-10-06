<template>
  <div class="history-container">
    <ChatList />
  </div>
</template>

<script setup>
import ChatList from './ChatList.vue';
</script>

<style scoped>
.history-container {
  flex: 1;
  overflow-y: auto;
  max-height: calc(100vh - 200px);
}
</style>
