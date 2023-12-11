<template>
  <div class="dropdown-menu">
    <div class="dropdown-menu-section dropdown-menu-profile-container">
      <div class="dropdown-menu-profile-info">
        <div class="centralizer">
          <div>
            <img
              class="rounded-profile-picture"
              src="https://media.licdn.com/dms/image/C4D03AQEvvcryxSyqIA/profile-displayphoto-shrink_200_200/0/1661438576706?e=1707955200&v=beta&t=sfqXhBRHZYj7PCISPa25sKrqdTCGmh6LVQG1xAiqwpE"
            />
          </div>
          <div>
            <div class="dropdown-menu-section-tittle">Giuliano Maradei</div>
            <div class="dropdown-menu-profile-headline">
              Software Engenier | Full-Stack | PHP | Laravel | Javascript |
              Vue.js | Nuxt
            </div>
          </div>
        </div>
        <button class="view-profile-button">View Profile</button>
      </div>
    </div>

    <div class="dropdown-menu-divisor"></div>

    <div class="dropdown-menu-section dropdown-menu-account-container">
      <div class="dropdown-menu-section-tittle">Account</div>
      <a class="dropdown-menu-option"> Reactivate Premium</a>
      <a class="dropdown-menu-option"> Settings & Privacy</a>
      <a class="dropdown-menu-option"> Help</a>
      <a class="dropdown-menu-option"> Language</a>
    </div>

    <div class="dropdown-menu-divisor"></div>

    <div class="dropdown-menu-section dropdown-menu-manage-container">
      <div class="dropdown-menu-section-tittle">Manage</div>
      <a class="dropdown-menu-option"> Reactivate Premium</a>
      <a class="dropdown-menu-option"> Settings & Privacy</a>
      <a class="dropdown-menu-option"> Help</a>
      <a class="dropdown-menu-option"> Language</a>
    </div>

    <div class="dropdown-menu-divisor"></div>

    <div class="dropdown-menu-section">
      <a class="dropdown-menu-option">Sign out</a>
    </div>
  </div>
</template>

<style scoped>
.dropdown-menu {
  position: absolute;
  top: calc(100% + 1rem);
  right: 0;
  z-index: 100;

  display: flex;
  flex-direction: column;
  align-items: center;

  visibility: hidden;
  width: 16rem;
  background-color: white;
  border-radius: 0.5rem 0 0.5rem 0.5rem;
  box-shadow:
    0px 0px 0px 1px rgb(140 140 140/0.2),
    0px 4px 4px rgb(0 0 0/0.3);

  .dropdown-menu-section {
    width: 100%;
    padding: 0.5rem;
    box-sizing: border-box;

    .dropdown-menu-option {
      &:hover {
        text-decoration: underline;
      }

      font-size: 0.85rem;
    }

    .dropdown-menu-section-tittle {
      font-size: 1rem;
      font-weight: 600;
      color: black;
    }
  }

  .dropdown-menu-divisor {
    width: 100%;
    height: 1px;
    background-color: #666666;
  }

  .dropdown-menu-profile-container {
    color: black;
    display: flex;
    align-items: center;
    flex-direction: column;
    padding: 0.5rem;
    gap: 1rem;

    .dropdown-menu-profile-info {
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 0.5rem;

      .rounded-profile-picture {
        border-radius: 50%;
        width: 4rem;
        height: 4rem;
      }

      .dropdown-menu-profile-headline {
        font-size: 0.85rem;
        font-weight: 400;
      }

      .centralizer {
        display: flex;
        align-items: center;
        gap: 1rem;
      }

      .view-profile-button {
        width: 100%;
        border: 1px solid #0a66c2;
        color: #0a66c2;
        padding: 0.2rem;
        font-size: 1rem;

        background-color: white;
        border-radius: 1.6rem;
        font-weight: 600;

        cursor: pointer;

        &:hover {
          border: 2px solid #0a66c2;
          color: #0a66c2;
        }
      }
    }
  }

  .dropdown-menu-account-container {
    display: flex;
    flex-direction: column;
    gap: 0.5rem;
    align-content: flex-start;
    justify-content: flex-start;
  }

  .dropdown-menu-manage-container {
    display: flex;
    flex-direction: column;
    gap: 0.5rem;
    align-content: flex-start;
    justify-content: flex-start;
  }
}
</style>
