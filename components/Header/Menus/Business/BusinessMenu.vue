<template>
  <div class="side-menu-wrapper">
    <div
      ref="sideMenu"
      tabindex="1"
      @focus="disableScroll"
      @blur="enableScroll"
      class="side-menu-container"
    >
      <div>
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
          <path
            d="M3 3h4v4H3zm7 4h4V3h-4zm7-4v4h4V3zM3 14h4v-4H3zm7 0h4v-4h-4zm7 0h4v-4h-4zM3 21h4v-4H3zm7 0h4v-4h-4zm7 0h4v-4h-4z"
          ></path>
        </svg>
      </div>

      <div class="menu-button">For Business ▾</div>
      <BusinessSideMenu :sideMenu="sideMenu" />
    </div>
    <div class="background-blur" />
  </div>
</template>

<script setup>
import { ref } from "vue";
import BusinessSideMenu from "~/components/Header/Menus/Business/BusinessSideMenu.vue";

const sideMenu = ref(null);
const disableScroll = () => {
  document.body.classList.add("disable-scroll");
};

const enableScroll = () => {
  document.body.classList.remove("disable-scroll");
  sideMenu.value.blur();
};
</script>

<style scoped>
.side-menu-wrapper {
  &:focus-within {
    & .background-blur {
      visibility: visible !important;
    }
  }
}

.side-menu-container {
  display: flex;
  flex-direction: column;
  align-items: center;

  &:focus-within {
    & .side-menu {
      right: 0 !important;
      visibility: visible !important;
    }

    & .background-blur {
      visibility: visible !important;
    }
  }
}

.menu-button {
  position: relative;
  background-color: transparent;
  border: none;
  outline: none;
  color: #666666;
  font-size: 0.8rem;

  &:hover {
    cursor: pointer;
    color: #191919;
  }
}

.background-blur {
  position: fixed;
  height: calc(100vh - 52px);
  width: 100vw;
  bottom: 0;
  left: 0;
  background-color: rgb(0 0 0 / 50%);
  visibility: hidden;
}
</style>
