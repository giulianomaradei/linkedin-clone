<template>
  <div>
    <button class="white-button">
      <slot />
    </button>
  </div>
</template>

<style scoped>
.white-button {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  box-sizing: border-box;

  color: #5e5e5e;
  background-color: white;
  outline: 1px solid #404040;
  border: none;
  padding: 0.4rem 1rem;
  margin: 5px 0;
  border-radius: 1.6rem;
  font-weight: 600;
  font-size: 100%;

  cursor: pointer;

  &:hover {
    background-color: #ebebeb;
    outline: 2px solid #3b3b3b;
  }
}
</style>
<script setup lang="ts"></script>
