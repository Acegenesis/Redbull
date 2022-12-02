<script setup>
import HomePage from "./components/HomePage.vue";
import Jeux from "./components/Jeux.vue";
</script>

<template>
  <div class="container">
    <HomePage />
    <Jeux />
  </div>
</template>

<style scoped>
.container {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 100%;
}
</style>
