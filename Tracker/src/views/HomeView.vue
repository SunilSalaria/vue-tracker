<template>
 <header>
    <nav class="navbar navbar-expand-lg bg-light shadow-sm">
  <div class="container-fluid">    
    <router-link class="navbar-brand d-flex align-items-center" to="/home">
    <img class="tracker-logo-img-vue" height="40" src="../assets/img/tracker-logo.svg">
    <span class="tracker-logo-text-vue ms-2 fs-4 text-primary">TRACKER</span>
    </router-link>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavDropdown" aria-controls="navbarNavDropdown" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNavDropdown">
      <ul class="navbar-nav ms-auto">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="#">Home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">About</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Pricing</a>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
            Sunil Salaria
          </a>
          <ul class="dropdown-menu">
            <li><a class="dropdown-item" href="#">Profile</a></li>
            <li><a class="dropdown-item" href="#">Setting</a></li>
            <li><a class="dropdown-item" href="#">Logout</a></li>
          </ul>
        </li>
      </ul>
    </div>
  </div>
</nav>
 </header>
</template>

<script setup>

</script>

<style>
.tracker-logo-img-vue{
    
}
</style>