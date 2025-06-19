<script setup>
import StoredResources from './components/learningResource/StoredResources.vue';
import TheHeader from './layouts/TheHeader.vue';
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
  <div>
    <TheHeader title="Learning Resources" />
    <StoredResources :resources="storedResources" />
  </div>
</template>
