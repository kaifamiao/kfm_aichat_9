<template>
  <aside :class="['sidebar', { 'is-hidden': isMobile && !showSidebar }]">
    <NewChat />
    <HistoryContainer />
    <Setting />
  </aside>
</template>

<script setup>
import { ref, computed, onMounted } from 'vue';
import NewChat from './NewChat.vue';
import HistoryContainer from './HistoryContainer.vue';
import Setting from './Setting.vue';

const showSidebar = ref(true);
const isMobile = ref(false);

const checkIsMobile = () => {
  isMobile.value = window.innerWidth <= 768;
};

onMounted(() => {
  checkIsMobile();
  window.addEventListener('resize', checkIsMobile);
});
</script>

<style scoped>
.sidebar {
  width: 250px;
  background-color: #fafafa;
  display: flex;
  flex-direction: column;
}
.is-hidden {
  display: none;
}
</style>
