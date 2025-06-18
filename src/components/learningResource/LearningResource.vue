<script setup>
import { defineProps } from 'vue';
import '../../style/learningResource.css';
const props = defineProps({
  resource: {
    type: Object,
    required: true,
  },
});
</script>

<template>
  <li>
    <div>
      <header>
        <h3>{{ props.resource.title }}</h3>
        <button>Delete</button>
      </header>
      <p>{{ props.resource.description }}</p>
      <nav>
        <a :href="props.resource.link" target="_blank">View Resource</a>
      </nav>
    </div>
  </li>
</template>
