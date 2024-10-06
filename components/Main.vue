<template>
  <main class="main">
    <MainHeader @toggleSidebar="toggleSidebar" />
    <MainContent />
    <ChatInput />
  </main>
</template>

<script setup>
import MainHeader from './MainHeader.vue';
import MainContent from './MainContent.vue';
import ChatInput from './ChatInput.vue';
import { inject } from 'vue';

const toggleSidebar = inject('toggleSidebar');
</script>

<style scoped>
.main {
  flex: 1;
  display: flex;
  flex-direction: column;
}
</style>
