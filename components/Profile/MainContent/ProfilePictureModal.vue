<template>
  <div class="profile-image-modal" @click.self="toggleModal">
    <div class="modal-portrait">
      <img
        src="https://media.licdn.com/dms/image/C4E03AQHVQ7GSbHdh1w/profile-displayphoto-shrink_200_200/0/1658945401063?e=1707350400&v=beta&t=wTimZbqYVVS4ARgiJImno1DwiRQ_z9gQzF37w7igsuo"
      />
      <div @click="props.toggleModal" class="close-modal"><span>x</span></div>
    </div>
  </div>
</template>
<script setup>
const props = defineProps({
  toggleModal: {
    type: Function,
    required: true,
  },
});
</script>
<style scoped>
.profile-image-modal {
  position: fixed;
  top: 0;
  left: 0;
  width: 100vw;
  height: 100vh;
  background-color: rgba(0, 0, 0, 0.5);
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 200;

  & img {
    width: 25vw;
    height: 25vw;
    border-radius: 50%;
  }

  & .modal-portrait {
    position: relative;
    width: 40vw;
    height: 30vw;
    background-color: black;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  & .close-modal {
    position: absolute;
    top: 0;
    right: 0;
    font-size: 2rem;
    width: 2rem;
    height: 2rem;
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 10px;
    color: white;
    padding: 0.5rem;
    border-radius: 50%;
    cursor: pointer;

    &:hover {
      background-color: #3b3b3b;
    }
  }
}
</style>
