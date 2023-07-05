<template>
  <div @click="open" class="nav-opener" style="position: absolute; padding: 20px;">
    <div class="span"></div>
    <div class="span"></div>
    <div class="span"></div>
  </div>
  <div @click="close" class="overlay" style="position: fixed"></div>
  <nav id="nav">
    <div class="cancel" style="width: 100%; position: relative;">
      <span @click="close" style="font-size: 40px;position: absolute; right: 10px; top: 0px">X</span>
    </div>
    <div @click="close" class="overlay" style="position: fixed"></div>
    
    <div class="logo">
      <img src="../assets/images/musala_logo-removebg-preview.png" alt="">
    </div>
    
    <ul>
      <li class="active">Home</li>
      <li>Company</li>
      <li>Services</li>
      <li>About</li>
      <li>Contact</li>
    </ul>
    <button>Join Us</button>
  </nav>
</template>

<script setup>
  
const open = () =>{
  const nav = document.querySelector('#nav');
  const overlay = document.querySelector('.overlay');
  nav.style.transform = 'translateX(0)'

  overlay.style.display = 'block'

}

const close = () =>{
  const overlay = document.querySelector('.overlay');
  const nav = document.querySelector('#nav');

  nav.style.transform = 'translateX(-100%)';
  overlay.style.display = 'none'
}
 
</script>

<style scoped>

  nav{
    position: sticky;
    top: 0px;
    width: 100%;
    color: white;
    padding: 20px;
    z-index: 20;
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 20px;
    font-weight: 700;
    flex-wrap: wrap;
    background: hsla(189, 100%, 50%, 1);
    background: linear-gradient(90deg, hsla(189, 100%, 50%, 1) 0%, hsla(248, 16%, 61%, 1) 100%);
    background: -moz-linear-gradient(90deg, hsla(189, 100%, 50%, 1) 0%, hsla(248, 16%, 61%, 1) 100%);
    background: -webkit-linear-gradient(90deg, hsla(189, 100%, 50%, 1) 0%, hsla(248, 16%, 61%, 1) 100%);
    filter: progid: DXImageTransform.Microsoft.gradient( startColorstr="#01DBFF", endColorstr="#918DAC", GradientType=1 );
  }
  .logo{
   width: 70px
  }

  .overlay{
    width: 100vw;
    height: 100vh;
    display: none;
    background-color: rgba(0, 0, 0, 0.623);
  }

  .logo img{
    width: 100%
  }

  ul{
    display: flex;
    /* border: 1px solid; */
    flex-wrap: wrap;
    width: fit-content;
    gap: 20px;
    justify-content: space-around;
    list-style: none;
    max-width: 40%
  }

  .cancel{
    display: none;
  }

  ul li{
    padding: 5px
  }

  button{
    position: relative;
    width: 100px;
    max-width: 100px;
    padding: 10px;
    background-color: rgb(168, 217, 95);
    border-radius: 5px;
    border: none;
    cursor: pointer
  }

  .nav-opener{
    display: none
  }


  @media screen and (max-width: 700px){
    nav{
      border: 1px solid;
      min-height: 100vh;
      height: auto;
      position: fixed;
      min-width: 300px;
      width: 50%;
      flex-direction: column;
      justify-content: flex-start;
      align-items: center;
      gap: 50px;
      padding: 10px;
      transform: translateX(-100%);
      transition: .2s;
    }

    .logo{
      font-size: 3em;
      width: 70%;
      align-self: center;
    }

    ul{
      flex-direction: column;
      justify-content: center;
      align-items: center;
      gap: 10px;
      width: 100%;
      max-width: 100%;
    }

    ul li{
      font-size: 30px;    
      padding:0; 
    }

    button{
      width: 100%;
      padding: 30px;
      max-width: 100%;
      font-weight: bolder;
      padding: 20px;
      font-size: 25px;
    }

    .nav-opener{
      display: block
    }   
    
    .cancel{
      display: block;
      position: absolute;
      top: 0px;
      right: 0px;
    }

    button{
      position: relative;
      padding: 5px;
      margin: 10px 0px;
      width: 100%;
    }

   .nav-opener .span{
    width: 40px;
    height: 5px;
    background: white;
    margin-bottom: 9px;
   }
  }
</style>