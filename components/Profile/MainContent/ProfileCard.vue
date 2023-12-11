<template>
  <Card id="profile-card">
    <template v-slot:header>
      <img
        class="background"
        src="https://media.licdn.com/dms/image/D4E16AQHDEsCHPHekOw/profile-displaybackgroundimage-shrink_350_1400/0/1690325945656?e=1707350400&v=beta&t=zzOVWkNvVX4zFQMX4RonkDElDhZizpktUHSAjZ0LshE"
      />
    </template>

    <ProfilePictureModal v-if="isModalActive" :toggleModal="toggleModal" />

    <div class="profile">
      <div class="first-layer">
        <img
          @click="toggleModal"
          class="profile-image"
          src="https://media.licdn.com/dms/image/C4E03AQHVQ7GSbHdh1w/profile-displayphoto-shrink_200_200/0/1658945401063?e=1707350400&v=beta&t=wTimZbqYVVS4ARgiJImno1DwiRQ_z9gQzF37w7igsuo"
        />
        <NotificationToggler />
      </div>
      <div class="second-layer">
        <div>
          <div>
            <div class="profile-title">Nate Ward-Jones</div>
          </div>
          <div class="profile-headline">MAAT, ACCA, BSc (Hons)</div>
          <div class="profile-address">
            Birmingham, England, United Kingdom . <a>Contact info</a>
          </div>
          <div class="profile-connections">
            <span class="number">116</span> connections
          </div>
        </div>
        <div class="profile-details-container">
          <div class="profile-details">
            <img
              class="profile-details-image"
              src="https://media.licdn.com/dms/image/C4E0BAQHaT0cdmSpKFg/company-logo_100_100/0/1673379477461/onthegoaccountants_logo?e=1710374400&v=beta&t=-0VSgi0dEWdCcHNdvX8rmput0A-Mn8Au4eR59YDkSrQ"
            />
            <div class="profile-detail-tittle">On The Go Accountants</div>
          </div>
          <div class="profile-details">
            <img
              class="profile-details-image"
              src="https://media.licdn.com/dms/image/D4E0BAQGf9qxp8MiosA/company-logo_100_100/0/1688374207533/oxfordbrookes_logo?e=1710374400&v=beta&t=qrtgirgu7qoX-b622nKpUJ8iSCuC-4PZPIVERZeb4No"
            />
            <div class="profile-detail-tittle">Oxford Brookes University</div>
          </div>
        </div>
      </div>
      <div class="third-layer">
        <BlueButton>Message</BlueButton>
        <WhiteButton>More</WhiteButton>
      </div>
    </div>
  </Card>
</template>

<script setup>
import { reactive, ref } from "vue";
import ProfilePictureModal from "~/components/Profile/MainContent/ProfilePictureModal.vue";
import NotificationToggler from "~/components/Profile/MainContent/NotificationToggler.vue";

const isModalActive = ref(false);

const toggleModal = () => {
  isModalActive.value = !isModalActive.value;
  if (isModalActive.value) {
    document.body.classList.add("disable-scroll");
  } else {
    document.body.classList.remove("disable-scroll");
  }
};

</script>

<style scoped>
.background {
  width: 100%;
  box-sizing: border-box;
  border-radius: 0.8rem 0.8rem 0 0;
}

.profile {
  max-width: 100%;
  height: 50%;
}

.profile-image {
  border-radius: 50%;
  width: 160px;
  border: 5px solid white;
  margin-top: -114px;
  z-index: 4;
  position: relative;

  &:hover {
    cursor: pointer;
  }
}

.profile-title {
  font-size: 1.5rem;
  font-weight: 600;
  width: fit-content;
  border-radius: 5px;

  &:hover {
    cursor: pointer;
    background-color: #ebebeb;
  }
}

.profile-headline {
  font-size: 1rem;
  font-weight: 400;
}

.profile-address {
  font-size: 0.8rem;
  color: #666666;
  padding: 0.5rem 0;

  a {
    color: #0a66c2;
    text-decoration: none;
    font-weight: 600;
    font-size: 0.9rem;

    &:hover {
      cursor: pointer;
      text-decoration: underline;
    }
  }
}

.profile-connections {
  font-size: 0.9rem;
  color: #666666;
  padding: 0.5rem 0;

  .number {
    font-weight: 600;
  }
}

.first-layer {
  display: flex;
  justify-content: space-between;
}

.second-layer {
  display: flex;
  justify-content: space-between;
}

.profile-details-container {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}

.profile-details {
  display: flex;
  align-items: center;
  gap: 1rem;
  height: 2rem;

  & .profile-detail-tittle {
    font-size: 0.9rem;
    font-weight: 600;

    &:hover {
      cursor: pointer;
      color: #0a66c2;
      text-decoration: underline;
    }
  }
}

.profile-details-image {
  height: inherit;

  &:hover {
    cursor: pointer;
  }
}

.third-layer {
  display: flex;
  align-items: center;
  align-content: stretch;
  gap: 0.5rem;
}
</style>
