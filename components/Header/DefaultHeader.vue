<script setup>
import LinkedinIcon from "~/components/Header/Menus/LinkedinIcon.vue";
import NavbarMenu from "~/components/Header/Menus/NavbarMenu.vue";
import NavbarSearchBar from "~/components/Header/Menus/NavbarSearchBar.vue";
import ProfileDropdown from "~/components/Header/Menus/Profile/ProfileMenu.vue";
import BusinessSideMenu from "~/components/Header/Menus/Business/BusinessMenu.vue";
import ScrollInfo from "~/components/Header/ScrollInfo.vue";
</script>

<template>
  <header>
    <div class="container">
      <div class="navbar">
        <LinkedinIcon />
        <NavbarSearchBar />

        <NavbarMenu
          text="Home"
          svg="M23 9v2h-2v7a3 3 0 01-3 3h-4v-6h-4v6H6a3 3 0 01-3-3v-7H1V9l11-7z"
        />
        <NavbarMenu
          text="My Network"
          svg="M12 16v6H3v-6a3 3 0 013-3h3a3 3 0 013 3zm5.5-3A3.5 3.5 0 1014 9.5a3.5 3.5 0 003.5 3.5zm1 2h-2a2.5 2.5 0 00-2.5 2.5V22h7v-4.5a2.5 2.5 0 00-2.5-2.5zM7.5 2A4.5 4.5 0 1012 6.5 4.49 4.49 0 007.5 2z"
        />
        <NavbarMenu
          text="Jobs"
          svg="M17 6V5a3 3 0 00-3-3h-4a3 3 0 00-3 3v1H2v4a3 3 0 003 3h14a3 3 0 003-3V6zM9 5a1 1 0 011-1h4a1 1 0 011 1v1H9zm10 9a4 4 0 003-1.38V17a3 3 0 01-3 3H5a3 3 0 01-3-3v-4.38A4 4 0 005 14z"
        />
        <NavbarMenu
          text="Messaging"
          svg="M16 4H8a7 7 0 000 14h4v4l8.16-5.39A6.78 6.78 0 0023 11a7 7 0 00-7-7zm-8 8.25A1.25 1.25 0 119.25 11 1.25 1.25 0 018 12.25zm4 0A1.25 1.25 0 1113.25 11 1.25 1.25 0 0112 12.25zm4 0A1.25 1.25 0 1117.25 11 1.25 1.25 0 0116 12.25z"
        />
        <NavbarMenu
          text="Notifications"
          svg="M22 19h-8.28a2 2 0 11-3.44 0H2v-1a4.52 4.52 0 011.17-2.83l1-1.17h15.7l1 1.17A4.42 4.42 0 0122 18zM18.21 7.44A6.27 6.27 0 0012 2a6.27 6.27 0 00-6.21 5.44L5 13h14z"
        />

        <NavbarMenu>
          <div class="circle-profile-image-container">
            <img
              class="circle-profile-image"
              src="https://media.licdn.com/dms/image/C4D03AQEvvcryxSyqIA/profile-displayphoto-shrink_100_100/0/1661438576706?e=1707350400&v=beta&t=teI1gE2ew7s_aXV-qfa8AESzJZku7SFMjZ7Ikm3qV-c"
            />
          </div>
          <ProfileDropdown />
        </NavbarMenu>

        <div class="header-divisor" />

        <NavbarMenu>
          <BusinessSideMenu></BusinessSideMenu>
        </NavbarMenu>

        <NavbarMenu>
          <p class="reactivate-premium">Reactivate Premium</p>
        </NavbarMenu>
      </div>
    </div>

    <ScrollInfo />
  </header>
</template>

<style scoped>
.container {
  position: fixed;
  top: 0;

  display: flex;
  justify-content: center;
  align-items: center;
  width: 100vw;
  z-index: 200;
  max-height: 52px;
  background-color: white;
  outline: 1px solid rgb(140 140 140/0.2);
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.navbar {
  display: flex;
  align-items: center;
  justify-content: space-between;

  height: 100%;
  width: 72rem;
  max-width: 90vw;
  background-color: white;
  color: #666666;
}

.circle-profile-image {
  border-radius: 50%;

  max-height: 1.5rem;
  max-width: 1.5rem;
}

.circle-profile-image-container {
  max-height: 100%;
  max-width: 100%;
}

.header-divisor {
  height: 52px;
  width: 1px;
  background-color: rgb(140 140 140/0.2);
}

.reactivate-premium {
  max-width: 100px;
  text-align: center;
  color: darkgoldenrod;
  text-decoration: underline;
  font-size: 0.8rem;

  &:hover {
    color: #5c3b09;
  }
}
</style>
