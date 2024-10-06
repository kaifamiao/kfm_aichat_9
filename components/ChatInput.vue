<template>
  <div class="chat-input">
    <SelectList />
    <textarea v-model="message" placeholder="请输入消息..."></textarea>
    <button @click="sendMessage">发送</button>
  </div>
</template>

<script setup>
import { ref } from 'vue';
import SelectList from './SelectList.vue';

const message = ref('');

const sendMessage = () => {
  if (message.value.trim()) {
    // 发送消息的逻辑
    alert(`发送消息: ${message.value}`);
    message.value = '';
  }
};
</script>

<style scoped>
.chat-input {
  display: flex;
  align-items: center;
  padding: 10px;
  background-color: #eaeaea;
}
.chat-input textarea {
  flex: 1;
  margin: 0 10px;
  padding: 10px;
}
.chat-input button {
  padding: 10px 20px;
}
</style>
