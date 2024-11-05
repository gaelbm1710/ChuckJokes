<template>
  <div class="card h-100">
    <img :src="icon_url" class="card-img-top" alt="Chuck Norris Icon" />
    <div class="card-body">
      <p class="card-text">{{ value }}</p>
    </div>
  </div>
</template>

<script setup>
import { defineProps } from "vue";

const props = defineProps({
  icon_url: String,
  value: String,
});
</script>

<style scoped>
.card {
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  border-radius: 8px;
}
.card-img-top {
  width: 100px;
  height: 100px;
  object-fit: cover;
  margin: 15px auto 0;
}
.card-text {
  font-size: 1rem;
  text-align: center;
}
</style>
