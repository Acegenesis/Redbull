<template>
    <div class="connect">
        <h1>Formulaire</h1>
        <a class="" href="https://www.youtube.com/watch?v=dQw4w9WgXcQ">Enregistrez vous</a>
        <div class="bubble1">
            <input type="text" v-model="name" />
            <p1>Votre nom</p1>
            <p4>{{ name }}</p4>
        </div>
        
        <!-- enter your age -->
        <div class="bubble2 isDisable">
            <input type="number" placeholder="0.0" step="0.01" v-model="age" />
            <p2>Votre Ã¢ge</p2>
            <p4>{{ age }}</p4>
        </div>
        
        <!-- enter your email -->
        <div class="bubble1">
            <input type="email" v-model="email" />
            <p1>Votre email</p1>
            <p4>{{ email }}</p4>
        </div>
        
        <!-- enter your password -->
        <div class="bubble2">
            <input type="password" v-model="password" />
            <p2>Votre mot de passe</p2>
            <p4>{{ password }}</p4>
        </div>

        <!-- enter your password confirmation -->
        <div class="bubble1">
            <input type="password" v-model="passwordConfirmation" />
            <p2>Confirmation du mot de passe</p2>
        </div>        
    </div>
</template>

<script>


</script>

<style scoped>
.connect {
    width: 100vw;
    height: 100vh;
    position: relative;
}

.isDisabled {
    pointer-events: none;
}


h1 {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    font-weight: bold;
    animation: rainbowColor 0.5s infinite;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    margin-top: 60px;
    font-size: 100px;
    text-shadow: 8px 8px 0px #296FB0;
}

a {
    border-radius: 50px;
    padding: 10px;
    text-align: center;
    width: 300px;
    margin: 0 auto;
    animation: rainbowColor 0.2s infinite;
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    font-weight: bold;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    font-size: 30px;
}

.bubble1 {
    direction: rtl;
    border-radius: 50px;
    padding: 10px;
    width: 200px;
    margin: 0 auto;
    background-color: #005BAA;
    animation: move 2s ease infinite;
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    font-weight: bold;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    margin-left: 500px;
    text-align: center;
    color: #A5AAC1;
    font-size: 20px;
}

.bubble2 {
    border-radius: 50px;
    padding: 10px;
    width: 200px;
    margin: 0 auto;
    background-color: #005BAA;
    animation: move 2s ease infinite;
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    font-weight: bold;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    margin-right: 500px;
    text-align: center;
    color: #A5AAC1;
    font-size: 20px;
}


@keyframes move {
    0% {
        transform: translateX(0);
    }
    50% {
        transform: translateX(300px);
    }
    70% {
        transform: translateX(-100px);
    }
    100% {
        transform: translateX(0);
    }
}

@keyframes rainbowColor {
    0% {
        color: #FF0000;
        background-color: #0000FF;
    }
    25% {
        color: #FF7F00;
        background-color: #A5AAC1;
    }
    50% {
        color: #FFFF00;
        background-color: green;
    }
    75% {
        color: #00FF00;
        background-color: aqua;
    }
    100% {
        color: #0000FF;
        background-color: #FF0000;
    }
}


@keyframes move2 {
    0% {
        transform: translateY(0);
    }
    50% {
        transform: translateY(300px);
    }
    70% {
        transform: translateY(-100px);
    }
    100% {
        transform: translateY(0);
    }
}

</style>