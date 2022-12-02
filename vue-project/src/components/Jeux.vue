<template>
  <div class="jeux">
    <div class="circle1"></div>
    <div class="circle2"></div>
    <div class="circle3"></div>
    <div class="cards">
      <div class="items">
        <p>Nice coock bro</p>
      </div>
      <div class="items"></div>
      <div class="items"></div>
      <div class="items"></div>
      <div class="items"></div>
    </div>
    <div class="progress">
      <h2>Mort due aux MST 45%</h2>
      <div class="progress-bar"></div>
    </div>
    <div class="time">
      <img src="../assets/horoge.png" alt="time">
      <h2>Temps restant : 1:30</h2>
    </div>
    <div class="cards second"></div>
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
  background-color: #005BAA;
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
  background-color: #7C96BC;
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
  background-color: #F7D1CD;
  transition: all 0.3s ease-in-out;
}

.cards .items:hover {
  transform: translateY(-100px) scale(1.1);
}

.cards .items p {
  color: #296FB0;
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
  background-color: #5282B6;
  transform: translate(-50%, -50%);
}

.circle2 {
  position: absolute;
  top: 50%;
  left: 50%;
  width: 180px;
  height: 180px;
  border-radius: 50%;
  background-color: #005BAA;
  transform: translate(-50%, -50%);
}

.circle3 {
  position: absolute;
  top: 50%;
  left: 50%;
  width: 150px;
  height: 150px;
  border-radius: 50%;
  background-color: #5282B6;
  transform: translate(-50%, -50%);
}

.progress {
  position: absolute;
  bottom: 50px;
  right: 30px;
  width: 300px;
  height: 30px;
  border-radius: 20px;
  background-color: #5282B6;
  transform: translateY(-50%);
}

.progress .progress-bar {
  width: 150px;
  height: 30px;
  border-radius: 20px;
  background-color: #F7D1CD;
  transition: all 0.3s ease-in-out;
}

.progress h2 {
  left: 50%;
  top: -40px;
  transform: translateX(-50%);
  position: absolute;
  color: #F7D1CD;
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
  justify-content: center;
  gap: 10px;
}

.time img {
  width: 40px;
  height: 40px;
}

.second {
  
}

</style>
