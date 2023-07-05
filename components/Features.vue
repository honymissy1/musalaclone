<template>
    <div>
        <div class="container">
            <div class="content">
                <h1>ENTERPRISE <span style="color: skyblue">SOFTWARE</span> SERVICES</h1>
                <h3>Have a long-term partner next to you on the path of success</h3>
            </div>
            <div class="image">
                <img src="../assets/images/business.gif" alt="Business Feature">
            </div>
        </div>

        <div class="container-b">
            <div class="content">
                <h1>WE LIVE IT. OUR JOB. OUR PASSION.</h1>
                <h3>Be on the top with us</h3>
            </div>
            <div class="image">
                <img src="../assets/images/work.png" alt="Business Feature">
            </div>
        </div>

        <div class="container">
            <div class="content">
                <h1>NEXT GENERATION IT SOLUTIONS</h1>
                <h3>Turning technology into value with creativity and innovation</h3>
            </div>
            <div class="image">
                <img src="../assets/images/tech.gif" alt="Business Feature">
            </div>
        </div>

        <div style="position: relative; width: 70%; margin: 30px auto; height: auto; z-index: -3;">
            <h1 style="font-size: 20px; position: absolute; top: 10px; left: 10px; color: white; ">VALUES</h1>
            <img src="../assets/images/values.png" alt="" style="box-shadow: 1px 1px 5px black; width: 100%">
        </div>

        <div class="container-b">
            <div class="content">
                <h1>THE JOY OF SHARING</h1>
                <h3>Strong IT Community. Sustainable Environment. Happy People.</h3>
            </div>
            <div class="image">
                <img src="../assets/images/team.png" alt="Business Feature">
            </div>
        </div>

    </div>
</template>

<script setup>


</script>

<style scoped>
.container{
    display: flex;
    width: 70%;

    margin: 0px auto;
    justify-content: space-around;
    gap: 30px;
    align-items: center;
    flex-wrap:wrap-reverse;
}

.container-b{
    display: flex;
    width: 70%;
    flex-direction: row-reverse;
    margin: 50px auto;
    justify-content: space-around;
    gap: 30px;
    align-items: center;
    flex-wrap: wrap-reverse;
    
}

.content{
    min-width: 50%;
    width: 300px

}

.content h1{
    font-size: 33px;
    border-bottom: 2px solid skyblue;
    text-align: justify;
}

.content h3{
     color: rgb(110, 105, 105);
     text-align: justify;
}

.image{
    width: 300px;
}

.image img{
    min-width: 300px;
    width: 100%
}
</style>