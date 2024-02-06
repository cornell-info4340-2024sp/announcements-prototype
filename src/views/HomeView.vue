<script setup>
import { ref } from 'vue';
import InputAnnouncement from '@/components/InputAnnouncement.vue';
import Announcement from '@/components/Announcement.vue';

const announcement = ref();

function updateAnnouncement(text) {
  announcement.value = text;
}
</script>

<template>
  <main>
    <InputAnnouncement v-on:announcementPosted="updateAnnouncement"/>
    <Announcement v-bind:message="announcement"/>
  </main>
</template>
