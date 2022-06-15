<template>
<NavBar msg="Welcome to Your Vue.js App"/>
  <div class="container">

      <div class="row">
    
       <div id="boxColor" class="col-6 bg-primary p-5">

        <div class="b-example-divider"><h2 class="fw-normal text-center ">Grupos</h2></div>

        <div class="list-group w-auto" >
          <a href="#" class="list-group-item list-group-item-action d-flex gap-3 py-3" aria-current="true">
            <img src="@/assets/img/computador-48.png" alt="twbs" width="32" height="32" style="border: 1px solid black;" class="rounded-circle flex-shrink-0">
            <div class="d-flex gap-2 w-100 justify-content-between">
              <div>
            <h6 class="mb-1">Comunidade Tech </h6>
                <p class="mb-0 opacity-75">Thiago: Manos vcs n sab... <img src="@/assets/img/24-64.png" alt="twbs" width="28" height="28" style="border: 1px solid black;" class="rounded-circle flex-shrink-0"></p>
              </div>
              <small class="opacity-50 text-nowrap">3m atrás</small>
            </div>
            <img src="@/assets/img/menu.png" alt="twbs" width="24" height="24" class="flex-shrink-0">
          </a>
      
          <a href="#" class="list-group-item list-group-item-action d-flex gap-3 py-3" aria-current="true">
            <img src="@/assets/img/java-64.png" alt="twbs" width="32" height="32" style="border: 1px solid black;" class="rounded-circle flex-shrink-0">
            <div class="d-flex gap-2 w-100 justify-content-between">
              <div>
                <h6 class="mb-1">Javeiros</h6>
                <p class="mb-0 opacity-75">Rogerio: Na versao que eu usei el...</p>
              </div>
              <small class="opacity-50 text-nowrap">5m atrás</small>
            </div>
            <img src="@/assets/img/menu.png" alt="twbs" width="24" height="24" class="flex-shrink-0">
          </a>    
        </div>

       </div>
    
       <div id="boxColor" class="col-6 bg-primary p-5">

        <div class="b-example-divider"><h2 class="fw-normal text-center">Chats privados</h2></div>

        <div class="list-group w-auto" >
          <a href="#" class="list-group-item list-group-item-action d-flex gap-3 py-3" aria-current="true">
            <img src="@/assets/img/fernanda.png" alt="twbs" width="32" height="32" style="border: 1px solid black;" class="rounded-circle flex-shrink-0">
            <div class="d-flex gap-2 w-100 justify-content-between">
              <div>
                <h6 class="mb-1">Fernanda</h6>
                <p class="mb-0 opacity-75">Tudo bem se for em Java 1... <img src="@/assets/img/24-64.png" alt="twbs" width="28" height="28" style="border: 1px solid black;" class="rounded-circle flex-shrink-0"></p>
              </div>
              <small class="opacity-50 text-nowrap">5m atrás</small>
            </div>
            <img src="@/assets/img/menu.png" alt="twbs" width="24" height="24" class="flex-shrink-0">
            
          </a>
      
          <a href="#" class="list-group-item list-group-item-action d-flex gap-3 py-3" aria-current="true">
            <img src="@/assets/img/rogerio.png" alt="twbs" width="32" height="32" style="border: 1px solid black;" class="rounded-circle flex-shrink-0">
            <div class="d-flex gap-2 w-100 justify-content-between">
              <div>
                <h6 class="mb-1">Rogerio</h6>
                <p class="mb-0 opacity-75">Mano bora fazer o tra...</p>
              </div>
              <small class="opacity-50 text-nowrap">5m atrás</small>
            </div>
            <img src="@/assets/img/menu.png" alt="twbs" width="24" height="24" class="flex-shrink-0">
          </a>    
        </div>

       </div>
    
      </div>
    
     </div>


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
body {
  background: var(--cinza);
}
.list-group {
  max-width: 460px;
  margin: 4rem auto;
}

.form-check-input:checked + .form-checked-content {
  opacity: .5;
}

.form-check-input-placeholder {
  border-style: dashed;
}
[contenteditable]:focus {
  outline: 0;
}

.list-group-checkable .list-group-item {
  cursor: pointer;
}
.list-group-item-check {
  position: absolute;
  clip: rect(0, 0, 0, 0);
}
.list-group-item-check:hover + .list-group-item {
  background-color: var(--bs-light);
}
.list-group-item-check:checked + .list-group-item {
  color: #fff;
  background-color: var(--bs-blue);
}
.list-group-item-check[disabled] + .list-group-item,
.list-group-item-check:disabled + .list-group-item {
  pointer-events: none;
  filter: none;
  opacity: .5;
}

.list-group-radio .list-group-item {
  cursor: pointer;
  border-radius: .5rem;
}
.list-group-radio .form-check-input {
  z-index: 2;
  margin-top: -.5em;
}
.list-group-radio .list-group-item:hover,
.list-group-radio .list-group-item:focus {
  background-color: var(--bs-light);
}

.list-group-radio .form-check-input:checked + .list-group-item {
  background-color: var(--bs-body);
  border-color: var(--bs-blue);
  box-shadow: 0 0 0 2px var(--bs-blue);
}
.list-group-radio .form-check-input[disabled] + .list-group-item,
.list-group-radio .form-check-input:disabled + .list-group-item {
  pointer-events: none;
  filter: none;
  opacity: .5;
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
.b-example-divider{
  height: 3rem;
    background-color: rgb(255, 255, 255)!important;
    border: solid rgba(0, 0, 0, .15);
    border-width: 1px 0;
    border-radius: 5rem;
    box-shadow: inset 0 0.5em 1.5em rgb(0 0 0 / 10%), inset 0 0.125em 0.5em rgb(0 0 0 / 15%);
}
.bg-primary {
  border: 5px solid white;
  border-radius: 5rem;
  background-color: var(--roxo)!important;
}
.mb-1{
  text-align: left;
}
#boxColor{
  background-color: var(--roxo)!important;
}
</style>
