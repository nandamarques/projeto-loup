<template>
 <ModalMsg :ativa="ativaModalMsg"/>

  <router-view></router-view>
  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/font-awesome/4.5.0/css/font-awesome.min.css">
<a v-if="ativaIcone" @click="abrirModal" style="position:fixed;width:60px;height:60px;bottom:40px;right:40px;background-color:#5E17EB;color:white;border-radius:50px;text-align:center;font-size:30px;box-shadow: 1px 1px 2px #888;
  z-index:1000;">
<i style="margin-top:16px" :class="icone"></i>
</a>
</template>

<script>
import ModalMsg from '@/components/ModalMsg.vue'

export default {
  data() {
    return {
      page: null,
      iconeSino: 'fa fa-bell',
      iconeClose: 'fa fa-close',
      icone: 'fa fa-bell',
      ativaModalMsg: false,
      ativaIcone: true,
    }
  },
  components: {
    ModalMsg
  },
  methods: {
    abrirModal() {
      if(this.ativaModalMsg == false) {
        this.icone = this.iconeClose
        this.ativaModalMsg = true
      } else {
        this.icone = this.iconeSino
        this.ativaModalMsg = false
      }      
    }
},
  watch: {
    '$route.name' (value) {
      if(value === 'home' || value === 'perfil') {
        this.ativaIcone = false
      }else{
        this.ativaIcone = true
      }
    }
  }

}
</script>
<style>
:root{
  --roxo: #5E17EB;
  --cinza: rgb(174, 172, 172);
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  height: 100vh;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
