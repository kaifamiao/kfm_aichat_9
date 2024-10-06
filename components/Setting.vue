<template>
  <div class="setting">
    <button @click="openModal">设置</button>
    <SettingModal v-if="showModal" @close="closeModal" />
  </div>
</template>

<script setup>
import { ref } from 'vue';
import SettingModal from './SettingModal.vue';

const showModal = ref(false);

const openModal = () => {
  showModal.value = true;
};

const closeModal = () => {
  showModal.value = false;
};
</script>

<style scoped>
.setting {
  padding: 10px;
}
.setting button {
  width: 100%;
  padding: 10px;
  font-size: 16px;
}
</style>
