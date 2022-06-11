<template>
 <ModalMsg :ativa="ativaModalMsg"/>

  <router-view></router-view>
  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/font-awesome/4.5.0/css/font-awesome.min.css">
<a @click="abrirModal" style="position:fixed;width:60px;height:60px;bottom:40px;right:40px;background-color:#5E17EB;color:white;border-radius:50px;text-align:center;font-size:30px;box-shadow: 1px 1px 2px #888;
  z-index:1000;">
<i style="margin-top:16px" class="fa fa-bell"></i>
</a>
</template>

<script>
import ModalMsg from '@/components/ModalMsg.vue'

export default {
  data() {
    return {
      ativaModalMsg: false
    }
  },
  components: {
    ModalMsg
  },
  methods: {
    abrirModal() {
      if(this.ativaModalMsg == false) {
        this.ativaModalMsg = true
      } else {
        this.ativaModalMsg = false
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
