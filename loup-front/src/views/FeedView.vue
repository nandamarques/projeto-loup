<template>
<NavBar msg="Welcome to Your Vue.js App"/>
  <main>
    
    <div class="topMenu">
        <button href="#" class="btn btn-light my-2">Todos</button>
        <button href="#" class="btn btn-light my-2">Tops semana</button>
        <button href="#" class="btn btn-light my-2">Popular</button>
        <button href="#" class="btn btn-light my-2">Aleatorio</button>
        <div class="my-2">
          <input type="search"  placeholder="Search" aria-label="Search">
          <button class="btn btn-light" style="margin-left: 25px;" type="submit">Search</button>
        </div>
                
    </div>
    
    <div class="album py-5 bg-light">
      <div class="container">
        <div class="row row-cols-1 row-cols-sm-2 row-cols-md-4 g-4">
          <!-- Começo do card -->
          <div class="col">
            <div class="card shadow-sm">
              <div width="100%" height="225">
                <img src="../assets/img/Medicina.jpeg" class="card-img-top" alt="">
              </div>
              <img src="" alt="">
              <div class="card-body">
                <strong>Medicina</strong>
                <div class="d-flex justify-content-between align-items-center">
                <p class="card-text">Profissionais</p>

                  <small class="text-muted"></small>
                  <div class="btn-group">
                    <small class="text-muted">20/30</small>
                  </div>
                </div>
                <div class="d-flex justify-content-between align-items-center">
                  <small class="text-muted"></small>
                  <div class="btn-group">
                    <button type="button" class="btn btn-sm btn-success"><img src="../assets/img/flecha.png"  width="70%"></button>
                  </div>
                  
                </div>
              </div>
            </div>
          </div>
          <!-- Fim do card -->

        </div>
      </div>
    </div>
    
  </main>
  
  <footer class="text-muted py-5">
    <div class="container">
      <p class="float-end mb-1">
        <a href="#">Back to top</a>
      </p>
      <p class="mb-1">Album example is &copy; Bootstrap, but please download and customize it for yourself!</p>
      <p class="mb-0">New to Bootstrap? <a href="/">Visit the homepage</a> or read our <a href="../getting-started/introduction/">getting started guide</a>.</p>
    </div>
  </footer>
</template>
<script>
import NavBar from '@/components/NavBar.vue'
export default {
  name: 'FeedView',
  components: {
    NavBar
  }
}
</script>

<style>
:root{
    --roxo: #5E17EB;
    --cinza: rgb(174, 172, 172);
}
.bg-light {
    --bs-bg-opacity: 1;
    background-color:var(--cinza);
}
.topMenu{
    background-color: var(--roxo);
    width: 100%!important;
}
.btn-light {
    color: var(--roxo)!important;
    border: 1px solid black!important;
    margin: 5px;
}
.btn-light:hover {
    color: white!important;
    background-color: var(--roxo)!important;
    border: 2px solid white!important;
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
  
  .b-example-divider {
    height: 3rem;
    background-color: rgba(0, 0, 0, .1);
    border: solid rgba(0, 0, 0, .15);
    border-width: 1px 0;
    box-shadow: inset 0 .5em 1.5em rgba(0, 0, 0, .1), inset 0 .125em .5em rgba(0, 0, 0, .15);
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
</style>
