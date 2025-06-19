<script setup>
import LearningResource from './LearningResource.vue';
import { defineProps } from 'vue';
defineProps({
  resources: {
    type: Array,
    required: true,
  },
});
</script>
<template>
  <ul>
    <LearningResource
      v-for="resource in resources"
      :key="resource.id"
      :resource="resource"
    />
  </ul>
</template>
