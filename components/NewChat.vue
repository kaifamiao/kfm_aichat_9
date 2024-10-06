<template>
  <div class="new-chat">
    <button @click="startNewChat">新建聊天</button>
  </div>
</template>

<script setup>
const startNewChat = () => {
  // 新建聊天的逻辑
  alert('新建聊天');
};
</script>

<style scoped>
.new-chat {
  padding: 10px;
}
.new-chat button {
  width: 100%;
  padding: 10px;
  font-size: 16px;
}
</style>
