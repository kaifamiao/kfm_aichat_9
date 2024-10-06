<template>
  <div class="main-content">
    <component :is="currentComponent" />
  </div>
</template>

<script setup>
import { ref } from 'vue';
import Chat from './Chat.vue';
import HistoryChat from './HistoryChat.vue';

// 根据需要切换组件
const currentComponent = ref('Chat');
</script>

<style scoped>
.main-content {
  flex: 1;
  overflow-y: auto;
  padding: 15px;
  background-color: #fff;
}
</style>
