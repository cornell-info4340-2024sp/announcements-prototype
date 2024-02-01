<script setup>
import InputCount from '@/components/InputCount.vue';
import Count from '@/components/Count.vue';

import { ref } from 'vue';

const count = ref(0);
</script>

<template>
  <main>
    <InputCount v-on:increase-by="count++" />
    <Count />
    {{  count }}
  </main>
</template>
