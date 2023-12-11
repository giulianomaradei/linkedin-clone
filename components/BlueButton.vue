<template>
  <div>
    <button class="blue-button">
      <slot></slot>
    </button>
  </div>
</template>

<style scoped>
.blue-button {
  padding: 0.4rem 1rem;
  margin: 5px 0;
  border-radius: 1.6rem;
  font-weight: 600;
  font-size: 100%;

  background-color: #0a66c2;
  color: white;
  border: none;

  &:hover {
    background-color: #004182;
    cursor: pointer;
  }

  &:active {
    background-color: #092440;
  }
}
</style>
