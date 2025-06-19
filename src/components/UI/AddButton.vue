<template>
  <button class="add-button"><slot /></button>
</template>
<style scoped>
.add-button {
  background-color: #ffa600;
  color: white;
  padding: 8px 16px;
  border: none;
  border-radius: 6px;
  cursor: pointer;
}
.add-button:hover {
  background-color: #e59400;
}
</style>
