<template>
  <div class="home-page">
    <div class="home-page__title">
      <h1>PHodozer</h1>
    </div>
    <div class="home-page__button">
      <a>Jouer</a>
    </div>
  </div>

</template>

<script>

export default {
  name: 'HomePage',
};

</script>

<style>
.home-page {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 100vw;
}

.home-page__title {
  font-size: 5rem;
  font-weight: 700;
  color: #fff;
  margin-bottom: 50px;
}

.home-page__button a {
  padding: 20px;
  border-radius: 0.5rem;
  font-size: 30px;
  background-color: rgb(0 189 126 / 0.5);
  color: #fff;
}

.home-page__button {
    transition: all 0.3s ease;
}
.home-page__button:hover {
  transform: scale(1.5);
}

.home-page__button a:hover {
  background-color: rgb(0 189 126);

}
</style>
