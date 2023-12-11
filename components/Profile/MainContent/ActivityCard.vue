<template>
  <Card>
    <div class="activity-container">
      <div>
        <div class="section-title">Activity</div>
        <div class="followers">116 followers</div>
      </div>

      <div class="info">
        <strong>Nate Ward-Jones</strong> reposted this • 8mo
      </div>
      <img
        width="64"
        src="https://media.licdn.com/dms/image/D4E22AQF9727EhnFK0Q/feedshare-shrink_160/0/1681299287842?e=1704931200&amp;v=beta&amp;t=INlWTEOe4g6h6VPwQyv6qClXXSBV1CEQ0i_N4rDa7s4"
        loading="lazy"
        height="64"
        alt="No alternative text description for this image"
        id="ember499"
        class="ivm-view-attr__img--centered feed-mini-update-commentary__image evi-image lazy-image ember-view"
      />
      <p>(Reactions Icons)</p>
      <div class="comments-counter">1 comment</div>
    </div>

    <template v-slot:footer>
      <CardFooterButton>Show all posts -></CardFooterButton>
    </template>
  </Card>
</template>

<script setup>
import Card from "~/components/Card.vue";
</script>

<style scoped>

.comments-counter{
  position: absolute;
  bottom: 0;
  right: 0;
  color: #666666;
  font-size: 0.8rem;
  padding: 1rem;
}

.activity-container {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}

.section-title {
  font-size: 1.3rem;
  font-weight: 600;
}

.followers {
  color: #666666;
}

.info {
  padding-top: 10px;
  font-size: 0.8rem;
  color: #666666;
}
</style>
