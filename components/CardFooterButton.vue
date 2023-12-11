<template>
  <div class="footer-button">
    <slot />
  </div>
</template>

<style scoped>
.footer-button {
  width: 100%;
  display: flex;
  justify-content: center;

  background-color: white;
  border-radius: 0 0 0.8rem 0.8rem;
  padding: 0.5rem 0;
  border-top: 1px solid #ebebeb;
  color: #666666;
  font-weight: 600;

  cursor: pointer;

  &:hover {
    background-color: #f3f3f3;
  }
}
</style>
