<template>
   <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
    <div class="col-1.5 ml-5 m-3">      
        <img class="logo d-flex justify-content-start" src="../../assets/Logo-Rayotec.png" alt="LogoRayo">       
    </div> 
 
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>

  <div class="collapse navbar-collapse" id="navbarSupportedContent">
    <ul class="navbar-nav mr-auto bg-dark">
      <li class="nav-item active">
        <a class="nav-link btn-lg btn-dark" href="#">Productos <span class="sr-only">(current)</span></a>
      </li>
      <li class="nav-item active">
        <a class="nav-link btn-lg btn-dark" href="#">Soluciones <span class="sr-only">(current)</span></a>
      </li>
      <li class="nav-item active">
        <a class="nav-link btn-lg btn-dark" href="#">Servicios</a>
      </li>
      <li class="nav-item active">
        <a class="nav-link btn-lg btn-dark" href="#">Asistencia</a>
      </li>
      <li class="nav-item active">
        <router-link :to="{name: 'catalogoProductos'}"> </router-link>
        <a class="nav-link btn-lg btn-dark" href="#">Almacen</a>
      </li>
      
    </ul>
   
  </div>
  <div class="collapse navbar-collapse" id="navbarSupportedContent">
    <ul class="navbar-nav mr-auto bg-dark">      
      <li class="nav-item active">
        <i class="bi bi-cart"></i>
      </li>
      
    </ul>
   
  </div>
</nav>
</template>
<script>
</script>
<style>
.logo{
  width:35%;

}
</style>