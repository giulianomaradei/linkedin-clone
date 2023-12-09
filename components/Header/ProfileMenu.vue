<template>
  <div class="profileMenu">
    <div class="circleProfileImage">
      <img class="circleProfileImage" src="https://media.licdn.com/dms/image/C4D03AQEvvcryxSyqIA/profile-displayphoto-shrink_100_100/0/1661438576706?e=1707350400&v=beta&t=teI1gE2ew7s_aXV-qfa8AESzJZku7SFMjZ7Ikm3qV-c">
    </div>
    <div>Me</div>
  </div>
</template>

<style>
  .profileMenu{
    display: flex;
    flex-direction: column;
    align-items: center;

    background-color: antiquewhite;
  }
  .circleProfileImage{
    height: 50px;
    width: 50px;
    border-radius: 50%;
    background-color: #c4c4c4;
  }
</style>
<script setup lang="ts">
</script>
