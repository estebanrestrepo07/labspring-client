<template>
    <nav class="navbar">
        <router-link to="/ingresar" class="navbar-brand" msg="daniel">Registrar trabajadores</router-link>
        <router-link to="/" class="navbar-brand">Lista de trabajadores</router-link>
                     

    </nav>
</template>

<script>
    export default {
        name: "navbar"
    }
</script>
<style>
.navbar{
    background-color: rgb(19, 19, 19);
}
.navbar .navbar-brand{
    color:rgb(255, 255, 255);
   
}
.navbar-brand:hover{
    color:rgb(18, 209, 34);
   
}
</style>