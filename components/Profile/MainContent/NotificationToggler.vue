<template>
  <div class="notification-container">
    <svg
        class="notification"
        @click="handleNotification"
        viewBox="-1 -1 24 24"
        xmlns="http://www.w3.org/2000/svg"
        height="24"
        width="24"
    >
      <path
          d="M18.791666666666664 16.041666666666664V10.083333333333332a7.791666666666666 7.791666666666666 0 0 0 -5.07925 -7.295749999999999 2.75 2.75 0 0 0 -5.4285 0A7.78525 7.78525 0 0 0 3.208333333333333 10.083333333333332v5.958333333333333a2.75 2.75 0 0 1 -2.75 2.75h21.083333333333332a2.75 2.75 0 0 1 -2.75 -2.75Z"
          :fill="notification.color"
          stroke="#666666"
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
      ></path>
      <path
          d="M13.75 18.791666666666664a2.75 2.75 0 1 1 -5.5 0"
          fill="none"
          stroke="#666666"
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
      ></path>
    </svg>
    <div class="notification-popup">{{ notification.popupMessage }}</div>
  </div>
</template>

<script setup>
import {reactive} from "vue";

const notification = reactive({
  color: "none",
  popupMessage: "Get notified about all of Nate’s posts.",
});

const handleNotification = () => {
  if (notification.color === "none") {
    notification.color = "gray";
    notification.popupMessage = "Only get notified about Nate’s top posts.";
  } else {
    notification.color = "none";
    notification.popupMessage = "Get notified about all of Nate’s posts.";
  }
};
</script>


<style scoped>
.notification-container {
  position: relative;

  &:hover {
    cursor: pointer;

    .notification-popup {
      opacity: 1;
    }
  }

  .notification {
    padding: 0.8rem;

    &:hover {
      cursor: pointer;
      background-color: #ebebeb;
      border-radius: 50%;
    }
  }

  .notification-popup {
    opacity: 0;
    position: absolute;
    top: 100%;
    left: 50%;
    transform: translateX(-50%);
    background-color: white;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    width: max-content;
    border: 1px solid #ebebeb;
    padding: 10px;
    border-radius: 0.8rem;
    z-index: 1;

    transition: opacity 0.3s ease-in-out;

    font-size: 0.9rem;
    color: #666666;
  }
}
</style>
