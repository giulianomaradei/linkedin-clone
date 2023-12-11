<template>
  <div class="dropdown-wrapper">
    <button class="dropdown-button">Me ▾</button>
    <ProfileDropdown />
  </div>
</template>

<script setup lang="ts">
import ProfileDropdown from "~/components/Header/Menus/Profile/ProfileDropdown.vue";
</script>

<style scoped>
.dropdown-wrapper {
  position: relative;

  &:focus-within {
    & .dropdown-menu {
      visibility: visible;
    }
  }
}

.dropdown-button {
  position: relative;
  background-color: transparent;
  border: none;
  outline: none;
  color: #666666;

  &:hover {
    cursor: pointer;
    color: #191919;
  }
}
</style>
