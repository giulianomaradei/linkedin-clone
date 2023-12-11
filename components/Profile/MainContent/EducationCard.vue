<template>
  <Card>
    <div class="section-tittle">Education</div>
    <div class="education-container">
      <div class="education">
        <div>
          <img
            class="company-logo"
            src="https://media.licdn.com/dms/image/D4E0BAQGf9qxp8MiosA/company-logo_100_100/0/1688374207533/oxfordbrookes_logo?e=1710374400&v=beta&t=qrtgirgu7qoX-b622nKpUJ8iSCuC-4PZPIVERZeb4No"
          />
        </div>

        <div>
          <a class="education-tittle">Oxford Brookes University</a>
          <div class="education-info">
            Bachelor's degree, Applied Accounting
          </div>
          <div class="education-dates">Nov 2021 - Sep 2022</div>
          <div class="education-more">Grade: Pass</div>
        </div>
      </div>
      <div class="education">
        <div>
          <img
            class="company-logo"
            src="https://media.licdn.com/dms/image/D4E0BAQFhiriQNuluqQ/company-logo_100_100/0/1682266192901/selftaught_logo?e=1710374400&v=beta&t=QHsdd36x_XShWDc8fbXhss--vCUKuGv1nKPEpFDyQKU"
          />
        </div>

        <div>
          <a class="education-tittle">Self-taught</a>
          <div class="education-info">ATT, Taxation</div>
          <div class="education-dates">Aug 2020 - Jan 2023</div>
          <div class="education-more">Grade: Pass</div>
        </div>
      </div>
    </div>

    <template v-slot:footer>
      <CardFooterButton>Show all 6 education</CardFooterButton>
    </template>
  </Card>
</template>

<script setup>
import Card from "~/components/Card.vue";
</script>

<style scoped>
.section-tittle {
  font-size: 1.3rem;
  font-weight: 600;
  padding: 0.5rem 0;
}

.education-container {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}

.education {
  display: flex;
  gap: 0.5rem;

  .education-tittle {
    font-weight: bold;

    &:hover {
      text-decoration: underline;
      cursor: pointer;
      color: #0a66c2;
    }
  }

  .education-info {
    font-size: 0.9rem;
    font-weight: 400;
  }

  .education-dates {
    font-size: 0.9rem;
    font-weight: 400;
    color: rgba(0, 0, 0, 0.6);
  }

  .education-more {
    font-size: 0.9rem;
    padding-top: 10px;
    font-weight: 400;
  }
}
</style>
