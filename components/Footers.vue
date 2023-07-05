<template>
    <footer>
      <header>CONTACTS</header>


      <div class="container">
        <div class="social"> 
          <img src="../assets/images/icon1.png" alt="" />
          <img src="../assets/images/icon2.png" alt="" />
          <img src="../assets/images/icon3.png" alt="" />
          <img src="../assets/images/icon4.png" alt="" />
        </div>
       <div class="card">
        <h1>SOFIA</h1>
        <p>World Trade Center 36, Dragan Tsankov blvd. Sofia 1057, Bulgaria</p>
        <div>
          <p>musala@musala.com</p>
          <p>+359 (2) 969 5821</p>
          <p>Fax +359 (2) 969 5822</p>
        </div>
       </div>

       <div class="card">
        <h1>BURGAS</h1>
        <p>3 Adam Mickiewicz str., office 5, Burgas 8000, Bulgaria</p>
        <div>
          <p>musala@musala.com</p>
          <p>+359 (2) 969 5821</p>
          <p>Fax +359 (2) 969 5822</p>
        </div>
       </div>

       <div class="card">
        <h1>RUSE</h1>
        <p>1 Aleksandrovska str., entrance 2, floor 2, Ruse 7000, Bulgaria</p>
        <div>
          <p>musala@musala.com</p>
          <p>+359 (2) 969 5821</p>
          <p>Fax +359 (2) 969 5822</p>
        </div>
       </div>

       <div class="card">
        <h1>SKOPJE</h1>
        <p>Soravia Center, 3 Filip II Makedonski Str., Skopje 1000, North Macedonia</p>
        <div>
          <p>musala@musala.com</p>
          <p>+359 (2) 969 5821</p>
          <p>Fax +359 (2) 969 5822</p>
        </div>
       </div>

       
       
  
  
  
      </div>
    </footer>


</template>

<script setup>

</script>

<style scoped>
  footer{
    height: auto;
    width: 100%;
    background-color: rgb(202, 225, 185);
  }

  header{
    font-size: 30px;
    background-color: black;
    color: white;
    width: fit-content;
    margin: 40px auto;
    padding: 10px 20px;
  }

  .container{
    display: flex;
    gap: 30px;
    flex-wrap: wrap;
    justify-content: space-around;
    /* border: 1px solid  */
  }

  .card{   
     max-width: 300px;
    flex: 1;
    /* box-shadow: 1px 1px 10px black; */
    padding: 20px;
    border-radius: 5px;
  }

  .card h1{
    /* background-color:white; */
    color: steelblue;
    /* text-align: center; */
  }
  .card p{
    margin: 20px 0px
  }

  .social{
    width: 70px;
    height: 100;
    border-radius:0px 50px 50px 0px;
    background-color: white;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 30px;
    padding: 30px
  }

</style>