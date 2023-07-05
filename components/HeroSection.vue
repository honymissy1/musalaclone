<template>
    <div class="hero-section">
        <div class="hero-content">
            <h1>NEXT GENERATION IT SOLUTIONS</h1>
            <h3>Turning technology into value with creativity and innovation</h3>
            <button>Explore</button>
        </div>
    </div>
</template>

<script setup>


</script>

<style scoped>
.hero-section{
    background-image: url('../assets/images/hero.jpg');
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    width: 100%;
    height: 70vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    padding: 20px
}

.hero-content{
    padding: 0px;
    color: white;
    width: fit-content;
    text-align: center;
    text-shadow: .5px .5px 3px black;
    width: 500px
}

.hero-content h1{
 
    font-weight: 800;
}

.hero-content h3{
  color: rgb(198, 243, 141);
}

button{
    padding: 5px;
    width: 100px;
    border: none;
    margin-top: 20px;
    font-weight: 700;
    border-radius: 5px;
    background-color: rgb(249,171,33);

}
</style>