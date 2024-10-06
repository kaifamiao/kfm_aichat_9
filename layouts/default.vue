<template>
  <div id="app">
    <Header />
    <div class="main-content-wrapper">
      <Sidebar />
      <Main />
    </div>
    <Footer />
  </div>
</template>

<script setup>
import Header from '~/components/Header.vue';
import Sidebar from '~/components/Sidebar.vue';
import Main from '~/components/Main.vue';
import Footer from '~/components/Footer.vue';
</script>

<style>
/* 可根据需要添加全局样式 */
</style>
