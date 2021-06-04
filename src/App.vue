<script setup>
import { ref, onBeforeUnmount, onMounted } from 'vue';
import Navbar from './components/Navbar.vue';
import { REFRESH_INTERVAL } from './constants';

const timer = setInterval(() => {
  location.reload();
}, REFRESH_INTERVAL);

onBeforeUnmount(() => {
  clearInterval(timer);
});
</script>

<template>
  <Navbar />
  <div class="app-reviews-container">
    <div class="elfsight-app-752a0a2b-fcbf-4e00-93d8-4f3cd12c0213"></div>
  </div>
</template>

<style>
.app-reviews-container {
  background-color: #1f2937;
  padding: 16px;
  padding-left: 32px;
  padding-right: 32px;
}

.eapps-widget-toolbar {
  display: none;
}

.LoadMoreButton__Component-sc-5z801y-1 {
  background-color: #ffffff !important;
}
</style>
