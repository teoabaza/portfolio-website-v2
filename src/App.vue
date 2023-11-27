<template>
  <div id="app">
    <nav-bar/>
    <div id="content">
      <RouterView />
    </div>
    <loading-overlay v-if="loading"/>
    <notification :title="notificationTitle" :text="notificationText"/>
  </div>
</template>

<script setup>
import NavBar from './components/NavBar.vue';
import Notification from './components/Notification.vue';
import { RouterView } from 'vue-router';
import LoadingOverlay from './components/LoadingOverlay.vue';
import { loading, notificationTitle, notificationText } from './hooks/globals';

</script>

<style scoped>
</style>
