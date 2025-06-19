<template>
  <button class="save-button"><slot /></button>
</template>
<style scoped>
.save-button {
  background-color: #007bff;
  color: white;
  padding: 8px 16px;
  border: none;
  border-radius: 6px;
  cursor: pointer;
}
.save-button:hover {
  background-color: #0056b3;
}
</style>
