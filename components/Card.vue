<template>
  <div class="card">
    <slot name="header"></slot>
    <div class="content">
      <slot />
    </div>
    <slot name="footer"></slot>
  </div>
</template>

<style scoped>
.card {
  width: 100%;
  border-radius: 0.8rem;
  position: relative;

  box-shadow: 0 0 0 1px rgb(140 140 140/0.2);
  background-color: white;
}

.content {
  background-color: white;
  border-radius: 0.8rem;
  padding: 1rem;
  position: relative;
}
</style>
<script setup lang="ts"></script>
