<template>
<div v-if="ativa" class="modal modal-alert position-static d-block bg-secondary py-5" tabindex="-1" role="dialog" id="modalChoice">
  <div class="modal-dialog" role="document">
    <h1 class="shadow p-3 mb-5 bg-white rounded">Notificações</h1>
    <div class="modal-content rounded-3 shadow">
      <!-- Incio da notficacaition -->
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
          <a href="#" class="list-group-item list-group-item-action d-flex gap-3 py-3" aria-current="true">
            <img src="@/assets/img/naruto-sorridente.jpg" alt="twbs" width="32" height="32" style="border: 1px solid black;" class="rounded-circle flex-shrink-0">
            <div class="d-flex gap-2 w-100 justify-content-between">
              <div>
                <h6 class="mb-1">Anime friends Brasil</h6>
                <p class="mb-0 opacity-75">Convidou você para participar do grupo</p>
              </div>
              <small class="opacity-50 text-nowrap">15m atrás</small>
            </div>
            <img src="@/assets/img/menu.png" alt="twbs" width="24" height="24" class="flex-shrink-0">
          </a>
          <a href="#" class="list-group-item list-group-item-action d-flex gap-3 py-3" aria-current="true">
            <img src="@/assets/img/zenitsu.jpg" alt="twbs" width="32" height="32" style="border: 1px solid black;" class="rounded-circle flex-shrink-0">
            <div class="d-flex gap-2 w-100 justify-content-between">
              <div>
                <h6 class="mb-1">Shaolin_Matador123</h6>
                <p class="mb-0 opacity-75">Te enviou um pedido de amizade</p>
              </div>
              <small class="opacity-50 text-nowrap">21m atrás</small>
            </div>
            <img src="@/assets/img/menu.png" alt="twbs" width="24" height="24" class="flex-shrink-0">
          </a>
          <a href="#" class="list-group-item list-group-item-action d-flex gap-3 py-3" aria-current="true">
            <img src="@/assets/img/sonic-feio.jpg" alt="twbs" width="32" height="32" style="border: 1px solid black;" class="rounded-circle flex-shrink-0">
            <div class="d-flex gap-2 w-100 justify-content-between">
              <div>
                <h6 class="mb-1">Sonic_Feio_Original3142</h6>
                <p class="mb-0 opacity-75">Opa, Mano cê vai hoje ?</p>
              </div>
              <small class="opacity-50 text-nowrap">1m atrás</small>
            </div>
            <img src="@/assets/img/menu.png" alt="twbs" width="24" height="24" class="flex-shrink-0">
          </a>
          <a href="#" class="list-group-item list-group-item-action d-flex gap-3 py-3" aria-current="true">
            <img src="@/assets/img/celfie.jpg" alt="twbs" width="32" height="32" style="border: 1px solid black;" class="rounded-circle flex-shrink-0">
            <div class="d-flex gap-2 w-100 justify-content-between">
              <div>
                <h6 class="mb-1">Galerinha do Balacobaco</h6>
                <p class="mb-0 opacity-75">Sonic_Feio: enviou uma imagem no grupo</p>
              </div>
              <small class="opacity-50 text-nowrap">20m atrás</small>
            </div>
            <img src="@/assets/img/menu.png" alt="twbs" width="24" height="24" class="flex-shrink-0">
          </a>
          <a href="#" class="list-group-item list-group-item-action d-flex gap-3 py-3" aria-current="true">
            <img src="@/assets/img/Stranger_Things_logo.png" alt="twbs" width="32" height="32" style="border: 1px solid black;" class="rounded-circle flex-shrink-0">
            <div class="d-flex gap-2 w-100 justify-content-between">
              <div>
                <h6 class="mb-1">Bagulhos Sinistros (Teorias)</h6>
                <p class="mb-0 opacity-75">Convidou você para participar do grupo</p>
              </div>
              <small class="opacity-50 text-nowrap">1d atrás</small>
            </div>
            <img src="@/assets/img/menu.png" alt="twbs" width="24" height="24" class="flex-shrink-0">
          </a>
           <!-- Fim da notificoes -->
    </div>
  </div>
</div>
</template>
<script>
    export default {
      name: 'ModalMsg',
      props: {
        ativa: {
          type: Boolean,
          default: false
        }
      }
    }
</script>
<style scoped>
#modalChoice{
  background-color: white !important;
}
</style>