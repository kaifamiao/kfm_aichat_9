<template>
  <ul class="chat-list">
    <li v-for="chat in chats" :key="chat.id" @click="selectChat(chat)">
      {{ chat.title }}
    </li>
  </ul>
</template>

<script setup>
import { ref } from 'vue';

const chats = ref([
  { id: 1, title: '聊天记录1' },
  { id: 2, title: '聊天记录2' },
  { id: 3, title: '聊天记录3' },
  // 更多聊天记录...
]);

const selectChat = (chat) => {
  // 选择聊天的逻辑
  alert(`选择了${chat.title}`);
};
</script>

<style scoped>
.chat-list {
  list-style: none;
  padding: 0;
  margin: 0;
}
.chat-list li {
  padding: 10px;
  cursor: pointer;
  border-bottom: 1px solid #ddd;
}
.chat-list li:hover {
  background-color: #f0f0f0;
}
</style>
