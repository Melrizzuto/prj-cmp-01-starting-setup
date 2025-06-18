<script setup>
import LearningResource from './components/learningResource/LearningResource.vue';
import './style/app.css';
const storedResources = [
  {
    id: 'official-guide',
    title: 'Official Guide',
    description: 'The official Vue.js documentation and guide.',
    link: 'https://vuejs.org/guide/introduction.html',
  },
  {
    id: 'google',
    title: 'Google',
    description: 'Search the web with Google.',
    link: 'https://www.google.com',
  },
];
</script>

<template>
  <ul>
    <LearningResource
      v-for="resource in storedResources"
      :key="resource.id"
      :resource="resource"
    />
  </ul>
</template>
