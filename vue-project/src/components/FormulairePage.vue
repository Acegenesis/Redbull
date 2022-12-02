<template>
    <div class="connect">
        <h1>Formulaire</h1>
        <p>enregistrez vous</p>
        <div class="app__content">
        </div>
        <!-- enter your name -->
        <input type="text" v-model="name" />
        <p1>My name is</p1>
        <p1>{{ name }}</p1>
        
        <br />
        
        <!-- enter your age -->
        <input type="number" v-model="age" />
        <p1>I am</p1>
        <p1>{{ age }}</p1>
        
        <br />
        
        <!-- enter your email -->
        <input type="email" v-model="email" />
        <p1>My email is</p1>
        <p1>{{ email }}</p1>
        
        <br />
        
        <!-- enter your password -->
        <input type="password" v-model="password" />
        <p1>My password is</p1>
        <p1>{{ password }}</p1>
        
        <br />
        
        <!-- enter your password confirmation -->
        <input type="password" v-model="passwordConfirmation" />
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

h1 {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    font-weight: bold;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #A5AAC1;
    margin-top: 60px;
    font-size: 100px;
}

p {
    /* rounded box around the text */
    border-radius: 50px;
    padding: 10px;
    text-align: center;

    /* the box is the size of the text */
    width: 300px;

    /* center the box */
    margin: 0 auto;

    /* color of the box */
    background-color: #005BAA;

    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    font-weight: bold;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #A5AAC1;
    font-size: 30px;
}

/* footer */
.footer {
    position: fixed;
    left: 0;
    bottom: 0;
    width: 100%;
    background-color: #005BAA;
    color: white;
    text-align: center;
}

.p1 {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    font-weight: bold;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #A5AAC1;
    font-size: 20px;
}
</style>