<template>
  <div class="home-page">
    <div class="home-page__title">
      <h1 @click="fun">PH</h1><p>odozer</p>
    </div>
    <div class="home-page__button">
      <a @click="slide">Jouer</a>
    </div>
    <div class="home-page__button connection">
      <a @click="connect">Connexion</a>
    </div> 
    <audio id="audio" controls style="visibility: hidden;">
      <source src="../assets/sounds/pornhub.mp3" type="audio/mpeg" />
    </audio>
    
  </div>

</template>

<script>

export default {
  name: 'HomePage',
  methods: {
    fun: function fun() {
      var audio = document.getElementById("audio");
      audio.play();
    },
    slide: function slide() {
      document.getElementById("app").style.transform = "translateX(-100vw)";
    },
    connect: function connect() {
      document.getElementById("app").style.transform = "translateX(-200vw)";
    }

  }

};

</script>

<style>
.home-page {
  position: relative;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 100vw;
  height: 100vh;
}

.home-page__title {
  font-size: 5rem;
  font-weight: 700;
  color: #fff;
  margin-bottom: 80px;
  display: flex;
  align-items: center;
}

.home-page__title h1 {
  padding: 5px 20px;
  border-radius: 20px;
  font-weight: 700;
  background-color: orange;
  color: black;
  margin-right: 10px;
}


.home-page__button a {
  padding: 20px;
  border-radius: 0.5rem;
  font-size: 30px;
  background-color: orange;
  color: black;
  font-weight: 700;
}

.home-page__button {
    transition: all 0.3s ease;
}
.home-page__button:hover {
  transform: scale(1.5);
}

.home-page__button a:hover {
  background-color: orange;

}

.home-page__button.connection {
  position: absolute;
  top: 50px;
  right: 90px;
}


</style>
