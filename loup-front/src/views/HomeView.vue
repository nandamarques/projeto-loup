<template>
  <main class="form-signin w-100 m-auto">
    <b-alert v-if="teste">Default Alert</b-alert>
    <img
      class="mb-4"
      src="../assets/img/Loup.png"
      alt=""
      width="255"
      height="255"
    />
    <h1 class="h3 mb-3 fw-normal">Login</h1>
    <b-alert class="alert alert-danger" v-if="showDismissibleAlert">
      Login ou senha inválidos.
    </b-alert>
    <div class="form-floating">
      <input
        type="text"
        class="form-control"
        id="emailForm"
        placeholder="name@example.com"
        v-model="email"
      />
      <label for="emailForm">Email</label>
    </div>
    <div class="form-floating">
      <input
        type="password"
        class="form-control"
        id="senhaForm"
        placeholder="Password"
        v-model="senha"
      />
      <label for="senhaForm">Senha</label>
    </div>
    <div class="checkbox mb-3">
      <label> <input type="checkbox" value="remember-me" /> Lembrar-me </label>
    </div>
    <button class="w-100 btn btn-lg btn-primary" @click="login">Entrar</button>
    <p class="mt-5 mb-3 text-muted">&copy; UCSAL 2022–2022</p>
  </main>
</template>

<script>

export default {
  name: 'HomeView',
  components: {
  },
  data() {
    return {
      showDismissibleAlert: false,
      teste: false
    };
  },
  methods: {
    login() {
      if(this.email === "admin" && this.senha === "admin"){
        this.showDismissibleAlert = false;
        this.$router.push('/feed')
      }else{
        this.showDismissibleAlert = true;
      }
    },
  },
}
</script>
<style scoped>
@import url();
:root {
  --roxo: #5e17eb;
}
html,
body {
  height: 100%;
}

body {
  display: flex;
  align-items: center;
  padding-top: 40px;
  padding-bottom: 40px;
  background-color: #f5f5f5;
}

.form-signin {
  max-width: 330px;
  padding: 15px;
}

.form-signin .form-floating:focus-within {
  z-index: 2;
}

.form-signin input[type="email"] {
  margin-bottom: -1px;
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}

.form-signin input[type="password"] {
  margin-bottom: 10px;
  border-top-left-radius: 0;
  border-top-right-radius: 0;
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
  background-color: rgba(0, 0, 0, 0.1);
  border: solid rgba(0, 0, 0, 0.15);
  border-width: 1px 0;
  box-shadow: inset 0 0.5em 1.5em rgba(0, 0, 0, 0.1),
    inset 0 0.125em 0.5em rgba(0, 0, 0, 0.15);
}

.b-example-vr {
  flex-shrink: 0;
  width: 1.5rem;
  height: 100vh;
}

.bi {
  vertical-align: -0.125em;
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

.btn-primary {
  --bs-btn-color: #fff;
  --bs-btn-bg: var(--roxo);
  --bs-btn-border-color: #7b4bda;
  --bs-btn-hover-color: #fff;
  --bs-btn-hover-bg: #7b4bda;
  --bs-btn-hover-border-color: #7b4bda;
  --bs-btn-focus-shadow-rgb: 49, 132, 253;
  --bs-btn-active-color: #fff;
  --bs-btn-active-bg: #7b4bda;
  --bs-btn-active-border-color: #7b4bda;
  --bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
  --bs-btn-disabled-color: #fff;
  --bs-btn-disabled-bg: #7b4bda;
  --bs-btn-disabled-border-color: #7b4bda;
}
</style>
