<script setup>
import { defineProps } from 'vue';
import DeleteButton from './DeleteButton.vue';
import SaveButton from './SaveButton.vue';
import '../../style/baseButton.css';

const props = defineProps({
  variant: {
    type: String,
    default: 'standard',
  },
});

const componentsMap = {
  delete: DeleteButton,
  save: SaveButton,
};
</script>

<template>
  <component class="base-button" :is="componentsMap[props.variant]">
    <slot />
  </component>
</template>
