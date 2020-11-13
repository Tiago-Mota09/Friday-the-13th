<template>

  <div>

    <header>
      <div class="barra">
        <Menu @click="openMenu"/>
      <h1> Hoje é Sexta-Feira 13!</h1> 
        <img src="../assets/calendar.png" alt="" class="calendar"/>
      </div>
    </header>

    <div class="principal">
      
      <img
        src="../assets/mask.png"
        alt=""
        width="50px"
        class="mask"
      />
      <img 
      class="friday"
        src="../assets/friday.png"
        alt=""
      />&#x1F52A
      
    </div>
    
    <div class="content">
      
      <img
        src="../assets/foto1.jpg"
        alt="Jason foto 1"
        class="img"
      />
       <i class="material-icons">favorite share</i>

      <img
        src="../assets/foto2.jpg"
        alt="Jason foto 2"
         class="img"
      />
      <i class="material-icons">favorite share</i>

      <img
        src="../assets/foto3.jpg"
        alt="Jason foto 3"
         class="img"
      />
     <i class="material-icons">favorite share</i>

      <img
        src="../assets/foto4.jpg"
        alt="Jason foto 4"
         class="img"
      />
      <i class="material-icons">favorite share</i>
<!-- ==================================================================================== -->

      <img
        src="../assets/foto5.jpg"
        alt="Jason foto 5"
         class="img"
         width="350px"
      />
      <i class="material-icons">favorite share</i>

      <img
        src="../assets/foto6.jpg"
        alt="Jason foto 6"
         class="img"
         width="350px"
      />
      <i class="material-icons">favorite share</i>

      <img
        src="../assets/foto7.jpg"
        alt="Jason foto 7"
         class="img"
         width="350px"
      />
      <i class="material-icons">favorite share</i>

      <img 
      src="../assets/foto8.jpg" 
      alt="Halloween" 
       class="img"
       width="350px"
      />
      <i class="material-icons">favorite share</i>
<!-- ================================================================================== -->
      <img 
      src="../assets/gif.gif"
       alt="Halloween" 
       class="gif"
       />
      <i class="material-icons">favorite share</i>

      <img 
      src="../assets/mask.jpg" 
      alt="Halloween" 
      class="gifmask"
      />
      <i class="material-icons">favorite share</i>
    </div>
  </div>
</template>


<style>
*,
*::before,
*::after {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

.barra {
  height: 100px;
  width: 98.8%;
  font-family: "Trebuchet MS", "Lucida Sans Unicode", "Lucida Grande","Lucida Sans", Arial, sans-serif;
  color: white;
  font-size: 20px;
  background: rgb(117, 29, 29);
  box-shadow: 0 10px 5px rgb(51, 35, 35);
  border-radius: 5px;
  display: flex;
  align-items: center;
  justify-content: space-around;
  margin: 20px 10px 30px 70px;
}

/* ====================================================================== */

.calendar{
  box-shadow: none;
  padding-top: 30px;
}
.mask{
  box-shadow: none;
  padding-top: 30px;
}

/* ====================================================================== */

body {
  display: flex;
  background-color: rgb(110, 70, 70);
  padding-bottom: 100px;
  align-items: center;
}
.principal {
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 40px;
}
.friday{
  
  width: 250px;
  box-shadow: none;
  margin: 0;
}

img {
  max-width: 775px;
  height: auto;
  border-radius: 10px;
  box-shadow: 10px 10px 10px rgba(0, 0, 0, 0.849);
  margin: 0 10px 30px 10px;
}
.material-icons{
  color: rgb(160, 120, 120);
}
.gif{
width: 800px;
height: 440px;
}
.gifmask{
  width: 800px;
  height: 440px;
}

</style>

<script>
import Menu from '@/components/Menu'
export default {
    data:() => ({
      Menu: false
    }),
    components: {
        Menu 
    },
    openMenu(){
      this.Menu = true
    },
    resetMenu(){
      this.Menu = false
    },
}

</script>