<template>
  <div>
    <h2>Chuck Norris Jokes</h2>
    <ul>
      <li v-for="joke in jokes" :key="joke.value">{{ joke.value }}</li>
    </ul>
  </div>
</template>

<script setup>
import { ref } from "vue";

const jokes = ref([
  { value: "Chuck Norris can skydive into outer space." },
  { value: "The chief export of Chuck Norris is pain." },
  {
    value:
      "Chuck Norris doesn't read books. He stares them down until he gets the information he wants.",
  },
  { value: "Time waits for no man. Unless that man is Chuck Norris." },
  { value: "If you spell Chuck Norris in Scrabble, you win. Forever." },
]);
</script>

<style scoped>
h2 {
  font-size: 1.5rem;
  color: #333;
  text-align: center;
  margin-top: 1rem;
}
ul {
  list-style: none;
  padding: 0;
  display: flex;
  flex-direction: column;
  align-items: center;
}
li {
  background-color: #f3f3f3;
  padding: 1rem;
  margin: 0.5rem 0;
  border-radius: 5px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  width: 80%;
  max-width: 500px;
  text-align: center;
}
</style>
