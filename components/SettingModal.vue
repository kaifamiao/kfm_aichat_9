<template>
  <div class="modal-overlay" @click.self="close">
    <div class="modal-content">
      <h2>设置</h2>
      <p>这里是设置内容。</p>
      <button @click="close">关闭</button>
    </div>
  </div>
</template>

<script setup>
const close = () => {
  emit('close');
};
</script>

<style scoped>
.modal-overlay {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.5);
}
.modal-content {
  background-color: #fff;
  margin: 10% auto;
  padding: 20px;
  width: 80%;
  max-width: 500px;
}
</style>
