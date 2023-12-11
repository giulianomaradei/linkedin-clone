<template>
  <div class="navbar-button">
    <div v-if="props.svg">
      <svg
        class="icon"
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 24 24"
        fill="#666666"
        data-supported-dps="24x24"
        width="24"
        height="24"
        focusable="false"
      >
        <path :d="props.svg"></path>
      </svg>
    </div>

    <div v-if="props.img">
      <img :src="props.img" />
    </div>

    <span class="navbar-button-tittle" v-if="props.text">{{ props.text }}</span>
    <slot />
  </div>
</template>

<script setup>
const props = defineProps({
  svg: {
    type: String,
  },
  img: {
    type: String,
  },
  text: {
    type: String,
  },
});
</script>

<style scoped>
.navbar-button {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;

  height: inherit;
  min-width: 5rem;

  &:hover {
    cursor: pointer;

    & .icon {
      fill: #191919;
    }

    & .navbar-button-tittle {
      color: #191919;
    }
  }
}

.icon {
  max-height: 1.5rem;
  max-width: 1.5rem;
}

.navbar-button-tittle {
  font-size: 0.8rem;
}
</style>
