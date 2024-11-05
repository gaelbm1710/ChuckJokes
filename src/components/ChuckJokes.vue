<template>
  <div class="container">
    <h2>Chuck Norris Jokes</h2>
    <div class="row">
      <chuck-card
        v-for="joke in jokes"
        :key="joke.value"
        :icon_url="joke.icon_url"
        :value="joke.value"
        class="col-lg-4 col-md-6 col-sm-12 mb-4"
      />
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";
import ChuckCard from "./ChuckCard.vue";

const jokes = ref([
  {
    icon_url: "https://assets.chucknorris.host/img/avatar/chuck-norris.png",
    value: "Chuck Norris can skydive into outer space.",
  },
  {
    icon_url: "https://assets.chucknorris.host/img/avatar/chuck-norris.png",
    value: "The chief export of Chuck Norris is pain.",
  },
  {
    icon_url: "https://assets.chucknorris.host/img/avatar/chuck-norris.png",
    value:
      "Chuck Norris doesn't read books. He stares them down until he gets the information he wants.",
  },
  {
    icon_url: "https://assets.chucknorris.host/img/avatar/chuck-norris.png",
    value: "Time waits for no man. Unless that man is Chuck Norris.",
  },
  {
    icon_url: "https://assets.chucknorris.host/img/avatar/chuck-norris.png",
    value: "If you spell Chuck Norris in Scrabble, you win. Forever.",
  },
]);
</script>

<style scoped>
h2 {
  font-size: 1.5rem;
  color: #333;
  text-align: center;
  margin-top: 1rem;
}
</style>
