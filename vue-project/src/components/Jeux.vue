<template>
  <div class="jeux">
    <div class="Background"></div>
    <div class="cards my-cards"></div>
  </div>
</template>

<script>
export default {
  name: "JeuxPage",
};
</script>

<style>
.jeux {
  width: 100vw;
  height: 100vh;
  position: relative;
}

.cards {
  position: absolute;
  bottom: 0;
  left: 50%;
  transform: translateX(-50%);
  width: 50%;
  height: 150px;
  border-top-left-radius: 20px;
  border-top-right-radius: 20px;
  background-color: #7c96bc;
}

.Background {
  /* carré de couleur */
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: #005baa;
}
</style>
