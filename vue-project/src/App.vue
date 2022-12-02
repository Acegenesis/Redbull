<script setup>
import HomePage from "./components/HomePage.vue";
import Jeux from "./components/Jeux.vue";
import FormulairePage from "./components/FormulairePage.vue";
</script>

<template>
  <div class="container">
    <HomePage />
    <Jeux />
    <FormulairePage />

  </div>
</template>

<style scoped>
.container {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 100%;
}
</style>
