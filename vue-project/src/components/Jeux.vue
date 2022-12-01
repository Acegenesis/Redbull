<template>
  <div class="jeux">
    <div class="jeux__title">
      <h1>Jeux</h1>
    </div>
    <div class="jeux__button">
      <a href="https://www.youtube.com/watch?v=dQw4w9WgXcQ">Jouer</a>
    </div>
  </div>
</template>

<script>
export default {
  name: "JeuxPage",
};
</script>

<style>
.jeux {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 100vw;
  height: 100vh;
}

.jeux__title {
  font-size: 5rem;
  font-weight: 700;
  color: #fff;
  margin-bottom: 50px;
}

.jeux__button a {
  padding: 20px;
  border-radius: 0.5rem;
  font-size: 30px;
  background-color: rgb(0 189 126 / 0.5);
  color: #fff;
}

.jeux__button {
  transition: all 0.3s ease;
}

.jeux__button:hover {
  transform: scale(1.5);
}

.jeux__button a:hover {
  background-color: rgb(0 189 126);
}
</style>
