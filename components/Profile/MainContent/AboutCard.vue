<template>
  <Card style="position: relative">
    <div class="section-tittle">About</div>
    <div class="about-text" :class="{ seeMore: isCollapsed }">
      <span
        ><!---->&lt;&gt;Senior Accountant<!----><br /><br /><!---->&lt;&gt;Client
        finance manager at OTG
        <!----><br /><br /><!---->&lt;&gt;My role involves managing a portfolio
        of clients and assisting with monthly investor documents, managing month
        end process workflows and producing management reports alongside annual
        accounts preparation, CT600, accounts and CT600 reviews and creating
        finance processes for clients
        <!----><br /><br /><!---->&lt;&gt;Qualifications<!----><br /><!---->ACCA
        affiliate<!----><br /><!---->MAAT qualified
        <!----><br /><!---->BSc in Applied Accounting<!----><br /><!---->ATT
        passed (remaining exemptions TBC)<!---->
      </span>
      <button
        v-if="!isCollapsed"
        class="collapse-button"
        @click="isCollapsed = true"
      >
        ...see more
      </button>
    </div>
  </Card>
</template>

<script setup>
import { ref } from "vue";
import Card from "~/components/Card.vue";

const isCollapsed = ref(false);
</script>

<style scoped>
.seeMore {
  height: auto !important;
}

.collapse-button {
  position: absolute;
  right: 0;
  bottom: 0;
  background-color: transparent;
  border: none;
  color: rgb(0 0 0/0.6);
  font-size: 0.9rem;
  cursor: pointer;

  &:hover {
    color: #0a66c2;
  }
}

.about-text {
  position: relative;
  font-size: 0.9rem;
  line-height: 1.5rem;
  height: 5rem;
  overflow: hidden;
  text-overflow: ellipsis;
  margin: 0 auto;
}
</style>
