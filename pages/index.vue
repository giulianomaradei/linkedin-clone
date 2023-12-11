<template>
  <div class="content-container">
    <div class="centralizer">
      <main>
        <ProfileCard />
        <HighlightsCard />
        <AboutCard />
        <ActivityCard />
        <ExperienceCard />
        <EducationCard />
        <InterestsCard />
      </main>
      <aside>
        <LinkedinAd />
        <PeopleViewed />
        <MightLike />
      </aside>
    </div>

    <Footer />
  </div>
</template>

<script setup>
import ProfileCard from "~/components/Profile/MainContent/ProfileCard.vue";
import AboutCard from "~/components/Profile/MainContent/AboutCard.vue";
import ActivityCard from "~/components/Profile/MainContent/ActivityCard.vue";
import ExperienceCard from "~/components/Profile/MainContent/ExperienceCard.vue";
import EducationCard from "~/components/Profile/MainContent/EducationCard.vue";
import InterestsCard from "~/components/Profile/MainContent/InterestsCard.vue";
import LinkedinAd from "~/components/Profile/SideContent/LinkedinAd.vue";
import PeopleViewed from "~/components/Profile/SideContent/PeopleViewed.vue";
import MightLike from "~/components/Profile/SideContent/MightLike.vue";
import Footer from "~/components/Profile/Footer.vue";
import HighlightsCard from "~/components/Profile/MainContent/HighlightsCard.vue";
</script>

<style>
.company-logo {
  width: 48px;
}

.section-tittle {
  font-size: 1.3rem;
  font-weight: 600;
}
</style>

<style scoped>
.content-container {
  position: relative;
  width: 100vw;
  display: flex;
  padding: 1.5rem 0;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  margin-top: 52px;
}

.centralizer {
  width: 72rem;
  max-width: 90vw;
  display: flex;
  gap: 1rem;
}

main {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
  width: 50.25rem;
}

aside {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
  width: 18.75rem;
}
</style>
