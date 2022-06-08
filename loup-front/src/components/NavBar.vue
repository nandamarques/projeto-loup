<template>
  <nav class="navbar navbar-expand-md navbar-dark bg-dark mb-4">
  <div class="container-fluid">
    <router-link class="nav-link active" to="/feed"><img src="@/assets/img/Logo.png" alt="twbs" width="40" height="40" style="border: 1px solid black;" class="rounded-circle flex-shrink-0"/></router-link> 
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarCollapse" aria-controls="navbarCollapse" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarCollapse">
      <ul class="navbar-nav me-auto mb-2 mb-md-0">
        <li class="nav-item">
          <router-link class="nav-link active" to="/feed">Feed</router-link> 
        </li>
        <li class="nav-item">
          <router-link class="nav-link active" to="/conversas">Mensagens</router-link> 
        </li>
        <li class="nav-item">
          <a class="nav-link disabled">Disabled</a>
        </li>
      </ul>
      <form class="d-flex" role="search">
        <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
        <button class="btn btn-outline-success" type="submit">Search</button>
      </form>
    </div>
  </div>
</nav>
</template>
<script>
export default {
  name: 'NavBar',
  props: {
    msg: String
  }
}
</script>
<style>
.navbar {
  margin-bottom: 0px!important;
}
</style>