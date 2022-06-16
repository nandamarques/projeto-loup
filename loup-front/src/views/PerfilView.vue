<template>
<NavBar />

<main id="sessao">

  <section class="py-5 text-center container" >
    <div class="row py-lg-5">
      <div class="col-lg-6 col-md-8 mx-auto">
        <div class="container d-flex justify-content-center align-items-center">
             
             <div class="card">

              <div class="upper">

                <img src="../assets/img/Purpler.png" class="img-fluid">
                
              </div>

              <div class="user text-center">

                <div class="profile">

                  <img src="../assets/img/davi.png" class="rounded-circle" width="80">
                  
                </div>

              </div>


              <div class="mt-5 text-center">

                <h4 class="mb-0">Davi Silva</h4>
                <span class="text-muted d-block mb-2">Salvador - BA</span>

                <button class="btn btn-primary btn-sm follow">Follow</button>


                <div class="d-flex justify-content-between align-items-center mt-4 px-4">

                  <div class="stats">
                    <h6 class="mb-0">Amigos</h6>
                    <span>8,797</span>

                  </div>


                  <div class="stats">
                    <h6 class="mb-0">Projetos</h6>
                    <span>142</span>

                  </div>


                  <div class="stats">
                    <h6 class="mb-0">Ranques</h6>
                    <span>129</span>

                  </div>
                  
                </div>
                
              </div>
               
             </div>

        </div>
      </div>
    </div>
    <p class="shadow-lg p-3 mb-5 bg-white rounded">Desenvolvedor FullStack C# .Net | VueJs | Postgresql | </p>
  </section>

   <div class="album py-5 bg-light">
    <div class="container">
      <div class="shadow-lg p-3 mb-5 bg-white rounded">
        <div class="form-group">
          <label style="color: gray;" for="exampleFormControlTextarea1">O que você quer contar para os outros?</label>
          <textarea class="form-control" id="exampleFormControlTextarea1" rows="3"></textarea>
        </div>
        <br>
        <div class="imgs">
          <img src="../assets/img/camera-solid.svg" width="40" height="40" alt="">
          <img src="../assets/img/location-dot-solid.svg" width="40" height="40" alt="">
        </div>
        <button id="btnPublicar" class="btn btn-danger">Publicar</button>
      </div>
      <div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 g-3">
<!-- Inicio -->
        <div class="col">
            <img class="shadow-lg" src="../assets/img/davi1.png" width="60%" height="70%" alt="">
    
        </div>
<!-- Fim -->
<!-- Inicio -->
        <div class="col">
            <img class="shadow-lg" src="../assets/img/davi2.png" width="60%" height="70%" alt="">
            
        </div>
<!-- Fim -->
<!-- Inicio -->
        <div class="col">
            <img class="shadow-lg" src="../assets/img/davi3.png" width="60%" height="70%" alt="">
            
        </div>
<!-- Fim -->
<!-- Inicio -->
        <div class="col">
            <img class="shadow-lg" src="../assets/img/davi4.jpeg" width="60%" height="70%" alt="">
            
        </div>
<!-- Fim -->

      </div>
    </div>
  </div>

</main>
</template>
<script>
import NavBar from '@/components/NavBar.vue'
export default {
  name: 'PerfilView',
  components: {
    NavBar
  }
}
</script>

<style scoped>

:root{
  --roxo: #5E17EB;
  --cinza: rgb(174, 172, 172);
}
.imgs{
  display: flex;
  align-items: center;
}
.imgs img{
  margin-right: 10px;
  cursor: pointer;
}
#btnPublicar{
  background-color: var(--roxo);
  color: white;
  border: none;
  border-radius: 5px;
  padding: 10px;
  font-size: 14px;
  font-weight: bold;
  cursor: pointer;
  float: right;
  transition: 0.7s;
}
#btnPublicar:hover{
  background-color: white;
  color: var(--roxo);
  transform: scale(1.2);
}
.col img{
  border: 5px solid white;
  border-radius: 4rem;
  transition: 0.7s;
}
.col img:hover{
  transform: scale3d(1.3, 1.3, 1.1);
}
#sessao{
  background-color: var(--roxo);
  margin: auto;
}
      .bd-placeholder-img {
        font-size: 1.125rem;
        text-anchor: middle;
        -webkit-user-select: none;
        -moz-user-select: none;
        user-select: none;
      }

      @media (min-width: 768px) {
        .bd-placeholder-img-lg {
          font-size: 3.5rem;
        }
      }

      .b-example-vr {
        flex-shrink: 0;
        width: 1.5rem;
        height: 100vh;
      }

      .bi {
        vertical-align: -.125em;
        fill: currentColor;
      }

      .nav-scroller {
        position: relative;
        z-index: 2;
        height: 2.75rem;
        overflow-y: hidden;
      }

      .nav-scroller .nav {
        display: flex;
        flex-wrap: nowrap;
        padding-bottom: 1rem;
        margin-top: -1px;
        overflow-x: auto;
        text-align: center;
        white-space: nowrap;
        -webkit-overflow-scrolling: touch;
      }

      @import url("https://fonts.googleapis.com/css2?family=Poppins:weight@100;200;300;400;500;600;700;800&display=swap");


       body{
        background-color:#545454;
        font-family: "Poppins", sans-serif;
        font-weight: 300;
       }


       .card{

        width: 380px;
        border: none;
        border-radius: 15px;
        padding: 8px;
        background-color: #fff;
        position: relative;
        height: 370px;
       }

       .upper{

        height: 100px;

       }

       .upper img{

        width: 100%;
        border-top-left-radius: 10px;
        border-top-right-radius: 10px;

       }

       .user{
        position: relative;
       }

       .profile img{

        
        height: 80px;
        width: 80px;
        margin-top:2px;

       
       }

       .profile{

        position: absolute;
        top:-50px;
        left: 38%;
        height: 90px;
        width: 90px;
        border:3px solid #fff;

        border-radius: 50%;

       }

       .follow{

        border-radius: 15px;
        padding-left: 20px;
        padding-right: 20px;
        height: 35px;
       }

       .stats span{

        font-size: 29px;
       }
    </style>
