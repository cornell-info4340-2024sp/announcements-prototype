<script setup>
import { ref } from 'vue';
const announcementText = ref();
</script>

<template>
  <input type="text" placeholder="Announcement" v-model="announcementText"/>
  <button
    v-on:click="$emit('announcementPosted', announcementText)">
  Post
  </button>
</template>

<style scoped>
</style>
