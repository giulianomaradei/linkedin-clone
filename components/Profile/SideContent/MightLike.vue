<template>
  <Card>
    <div class="container">
      <div class="tittle-container">
        <div class="tittle">You might like</div>
        <span class="info">Courses for you</span>
      </div>

      <div class="courses-container">
        <div class="course">
          <div>
            <img
              class="course-image"
              src="https://media.licdn.com/dms/image/D560DAQHW2Icmm-wL6g/learning-public-crop_60_100/0/1683147182761?e=1702900800&v=beta&t=U6RJrw8lO9h8m_ivZMOpVpJYTahnLrOlAYiMb73AWMw"
            />
          </div>
          <div class="course-info">
            <div class="course-tittle">
              Learning Vertex AI: MLOps with Google Cloud
            </div>
            <div class="course-description">Skills: MLOps, Vertex</div>
            <div class="course-duration">1h 38min</div>
            <WhiteButton>Save</WhiteButton>
          </div>
        </div>

        <div class="course">
          <div>
            <img
              class="course-image"
              src="https://media.licdn.com/dms/image/D4D0DAQHuPLU458tMfQ/learning-public-crop_60_100/0/1690401045109?e=1702900800&v=beta&t=wUJ5JLon_KUPokLN-fFjXg-LDQs8wIjyIo4PBhseRlY"
            />
          </div>
          <div class="course-info">
            <div class="course-tittle">Avoiding Implicit Bugs in C++</div>
            <div class="course-description">Skills: C++</div>
            <div class="course-duration">1h 52min</div>
            <WhiteButton>Save</WhiteButton>
          </div>
        </div>
      </div>
    </div>
    <template v-slot:footer>
      <CardFooterButton>Show All</CardFooterButton>
    </template>
  </Card>
</template>

<script setup>
import Card from "~/components/Card.vue";
</script>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.tittle-container {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  gap: 0.5rem;
}

.tittle {
  font-weight: 600;
}

.info {
  color: #5e5e5e;
  font-size: 0.85rem;
}

.courses-container {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.course {
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
  gap: 1rem;
}

.course-image {
  width: 48px;
}

.course-info {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}

.course-tittle {
  font-weight: 600;

  &:hover {
    cursor: pointer;
    color: #0a66c2;
    text-decoration: underline;
  }
}

.course-description {
  font-size: 0.9rem;
}

.course-duration {
  color: #5e5e5e;
  font-size: 0.85rem;
}
</style>
