<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Registro Trabajadores</router-link> |
      <router-link to="/listaTrabajadores">Lista Trabajadores</router-link>
    </div>
    <router-view/>
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #151516;
  
}

#nav {
  padding: 30px;
  background-color: #6fd4f3;
}

#nav a {
  font-weight: bold;
  color: #161718;
  text-decoration: none;
  
}


#nav a.router-link-exact-active {
  color: #f8fcf8;
}
h1{
 background: #68f191;
 font-weight: bold;
 font-family: Avenir, Arial;
 color: white;
}
#contenedor {
   position:relative;
    height:150px;
    width:800px;
    margin:0 auto;
    top:40px;
}
#contenedor .form-control{
  top:60px;
  left:60px;
  margin-top:30px;
}
.col-sm-10
{
  top:60px;
  left:70px;
   margin:0 auto;
  margin-top:30px;
  
}
</style>
