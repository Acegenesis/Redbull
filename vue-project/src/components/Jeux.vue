<template>
  <div class="jeux">
    <div class="circle1"></div>
    <div class="circle2"></div>
    <div class="circle3"></div>
    <div class="cards">
      <div class="items">
        <p>Que signifie VIH ? </p>
      </div>
      <div class="items"></div>
      <div class="items"></div>
      <div class="items"></div>
      <div class="items"></div>
    </div>
    <div class="cards second">
      <h3>Bot 1</h3>
      <div class="items">Virus de l'Immuno-déficience Humaine</div>
      <div class="items"></div>
    </div>
    <div class="cards tree">
      <h3>Bot 2</h3>
      <div class="items">virus de l'infidélité Humaine</div>
      <div class="items"></div>
    </div>
    <div class="cards forrrr">
      <h3>Bot 3</h3>
      <div class="items">Variation de l'Immuno-Déficience
      Habituelle</div>
      <div class="items"></div>
    </div>

    <div class="progress">
      <h2>Mort due aux MST 45%</h2>
      <div class="progress-bar"></div>
    </div>
    <div class="time">
      <img src="../assets/horoge.png" alt="time">
      <h2>Temps restant : {{(Math.round(compteur/60) + " min " + Math.round(compteur%60))}} </h2>
    </div>
    <div class="param">
      <img src="../assets/parametres.png" alt="param" />
    </div>
    <div class="logo">
      <a @click="back">
        <img src="../assets/logoph.png" alt="logo" />
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: "JeuxPage",
  data() {
    return {
      compteur: 300,
    };
  },
  methods: {
    back: function back() {
      document.getElementById("app").style.transform = "translateX(0vw)";
    },
    comptdown() {
      let timer = setInterval(() => {
        this.compteur--;
        if (this.compteur === 0) {
          stop()
        }
      }, 1000);
    },
  },
  created() {
    this.comptdown();
  },

};


</script>

<style>
.logo img {
  position: absolute;
  top: 0;
  left: 0;
  width: 250px;
  margin: 20px;
}

.param img {
  width: 90px;
  height: 90px;
  position: absolute;
  top: 10px;
  right: 10px;
}

.jeux {
  width: 100vw;
  height: 100vh;
  position: relative;
  background-color: #005baa;
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
  display: flex;
  justify-content: center;
  gap: 20px;
}

.cards .items {
  transform: translateY(-50px);
  width: 130px;
  height: 180px;
  border-radius: 20px;
  padding: 10px;
  background-color: #f7d1cd;
  transition: all 0.3s ease-in-out;
}

.cards .items:hover {
  transform: translateY(-100px) scale(1.1);
}

.cards .items p {
  color: #296fb0;
  font-size: 12px;
  font-weight: 600;
}

.circle1 {
  position: absolute;
  top: 50%;
  left: 50%;
  width: 220px;
  height: 220px;
  border-radius: 50%;
  background-color: #5282b6;
  transform: translate(-50%, -50%);
}

.circle2 {
  position: absolute;
  top: 50%;
  left: 50%;
  width: 180px;
  height: 180px;
  border-radius: 50%;
  background-color: #005baa;
  transform: translate(-50%, -50%);
}

.circle3 {
  position: absolute;
  top: 50%;
  left: 50%;
  width: 150px;
  height: 150px;
  border-radius: 50%;
  background-color: #5282b6;
  transform: translate(-50%, -50%);
}

.progress {
  position: absolute;
  bottom: 50px;
  right: 30px;
  width: 300px;
  height: 30px;
  border-radius: 20px;
  background-color: #5282b6;
  transform: translateY(-50%);
}

.progress .progress-bar {
  width: 150px;
  height: 30px;
  border-radius: 20px;
  background-color: #f7d1cd;
  transition: all 0.3s ease-in-out;
}

.progress h2 {
  left: 50%;
  top: -40px;
  transform: translateX(-50%);
  position: absolute;
  color: #f7d1cd;
  font-size: 15px;
  font-weight: 700;
  width: 100%;
  text-align: center;
}

.time {
  position: absolute;
  bottom: 50px;
  left: 30px;
  width: 300px;
  height: 30px;
  border-radius: 20px;
  transform: translateY(-50%);
  display: flex;
  align-items: center;
  gap: 10px;
  font-size: 13px;
}

.time img {
  width: 40px;
  height: 40px;
}

.second,
.tree,
.forrrr {
  position: absolute;
  z-index: 9;
  top: 50px;
  left: 50%;
  transform: translateX(-50%) scale(0.5);
  border-radius: 20px;
}

.second .items,
.tree .items,
.forrrr .items {
  padding: 20px;
  transform: translateY(25%);
  color: #005baa;
}

.second .items:hover,
.tree .items:hover,
.forrrr .items:hover {
  transform: translateY(50px) scale(1);
}

.tree {
  top: 170px;
  right: 0px;
  transform: translateX(100px) scale(0.5) rotate(30deg);
}

.forrrr {
  top: 170px;
  left: 0px;
  transform: translateX(-100px) scale(0.5) rotate(-30deg);
}

.second h3,
.tree h3,
.forrrr h3 {
  position: absolute;
  top: -80px;
  left: 50%;
  transform: translateX(-50%);
  color: #f7d1cd;
  font-size: 40px;
  font-weight: 700;
  width: 100%;
  text-align: center;
}

.param:hover img {
  animation: tourne 0.4s ease-in-out infinite;
}

@keyframes tourne {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}

</style>


