<template>
  <div
    class="scroll-container"
    :class="{ visible: !targetIsVisible && profileCard }"
  >
    <div class="scroll-info">
      <div class="left-info">
        <img
          src="https://media.licdn.com/dms/image/C4E03AQHVQ7GSbHdh1w/profile-displayphoto-shrink_100_100/0/1658945401063?e=1707955200&v=beta&t=cj3P-glRL_M4GfFtSX9Vvl1yiDFGp0ybJjLhH_aJnA8"
        />
        <div class="profile-info">
          <div class="name">Nate Ward-Jones</div>
          <div class="headline">MAAT, ACCA, BSc (Hons)</div>
        </div>
      </div>
      <div class="right-info">
        <WhiteButton>More</WhiteButton>
        <BlueButton>Message</BlueButton>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";
import { useElementVisibility } from "@vueuse/core";

const profileCard = ref(null);
const targetIsVisible = useElementVisibility(profileCard);

onMounted(() => {
  profileCard.value = document.querySelector("#profile-card");
});
</script>

<style scoped>
.visible {
  top: 52px !important;
  box-shadow:
    0px 0px 0px 1px rgb(140 140 140/0.2),
    0px 4px 4px rgb(0 0 0/0.3);
}

.scroll-container {
  position: fixed;
  top: 0;

  display: flex;
  justify-content: center;
  align-items: center;
  width: 100vw;
  background-color: white;
  border-bottom: 1px solid rgb(140 140 140/0.2);

  margin: 0;
  padding: 4px;

  transition:
    top 0.5s ease-in-out,
    box-shadow 0.5s ease-in-out;
  z-index: 100;
}

.scroll-info {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 72rem;
  max-width: 90vw;
  height: 100%;
}

.profile-info {
  display: flex;
  flex-direction: column;
  gap: 0.2rem;
}

.left-info {
  display: flex;
  align-items: center;
  gap: 0.5rem;

  & .name {
    font-size: 0.9rem;
    font-weight: 600;
  }

  & .headline {
    font-size: 0.8rem;
    color: #666666;
  }

  & img {
    border-radius: 50%;
    max-height: 1.8rem;
    max-width: 1.8rem;
  }
}

.right-info {
  display: flex;
  gap: 0.5rem;
}
</style>
