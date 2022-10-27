<template>    
  <div id="app">  
    <NavBar /> 
    <Catalogo />  
  </div>  
  </template>    
  <script>  
   import NavBar from './views/Index/navBar.vue' 
   import Catalogo from './views/catalogoProductos/catalogoProductos.vue' 
  import Users from './components/Users.vue' 
  export default {    
  name: 'app',    
  components: {      
  Users,
  NavBar,
  Catalogo
  }  
  }  
  </script>    
  <style>  
  #app {    
  font-family: 'Avenir', Helvetica, Arial, sans-serif;    
  -webkit-font-smoothing: antialiased;    
  -moz-osx-font-smoothing: grayscale;    
  text-align: center;    
  color: #2c3e50;   
 
  }  
  </style>
