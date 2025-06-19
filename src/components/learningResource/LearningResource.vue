<script setup>
import { defineProps } from 'vue';
import BaseCard from '../UI/BaseCard.vue';
import BaseButton from '../UI/BaseButton.vue';
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
    <BaseCard class="learning-resource">
      <div class="card-content">
        <p>{{ props.resource.description }}</p>
        <a :href="props.resource.link" target="_blank">View Resource</a>
      </div>
      <div class="card-actions">
        <BaseButton variant="delete">Delete</BaseButton>
        <BaseButton variant="save">Save</BaseButton>
        <BaseButton variant="add">Add</BaseButton>
      </div>
    </BaseCard>
  </li>
</template>
