<template>
  <button class="delete-button"><slot /></button>
</template>
<style scoped>
.delete-button {
  background-color: #dc3545;
  color: white;
  padding: 8px 16px;
  border: none;
  border-radius: 6px;
  cursor: pointer;
}

.delete-button:hover {
  background-color: #c82333;
}
</style>
