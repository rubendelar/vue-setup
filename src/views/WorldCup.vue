<template>
  <div>
    <h1>{{ worldCupDates }}</h1>
  </div>
</template>

<script setup>
import { ref } from "vue";
const worldCupDates = ref(
  "The tournament kicks off on Sunday November 20 at the Al Bayt Stadium when Qatar take on Ecuador in Group A."
);
</script>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 1.2rem;
  top: -10px;
}
h2 {
  font-size: 2rem;
  font-weight: bold;
}
@media (min-width: 1024px) {
  div {
    min-height: 150px;
    display: flex;
    align-items: center;
    flex-direction: column;
    margin-top: 1px;
  }
}
</style>
