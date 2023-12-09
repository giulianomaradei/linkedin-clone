<template>
  <div class="navBarButton">
    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" data-supported-dps="24x24" fill="currentColor" class="mercado-match" width="24" height="24" focusable="false">
      <path :d="path"></path>
    </svg>
    <div>{{ text }}</div>
  </div>
</template>

<script setup>
  import { defineProps } from "vue";

  const props = defineProps({
    path: {
      type: String,
      required: true,
    },
    text: {
      type: String,
      required: true,
    },
  });

</script>

<style>
  .navBarButton{
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 5px;

    height: inherit;
    width: 100px;
    background-color: antiquewhite;
  }
</style>
