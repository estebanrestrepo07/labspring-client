<template>
  <div class="home">
    <h1>Registro de Trabajadores</h1>
    <div id="contenedor">
     
    <form>
  <div class="row">
    <div class="col">
      <input type="text" class="form-control" placeholder="Nombre">
    </div>
    <div class="col">
      <input type="text" class="form-control" placeholder="Apellido">
    </div>
  </div>
  <div class="row">
    <div class="col">
      <input type="text" class="form-control" placeholder="Numero de Cedula">
    </div>
    <div class="col">
      <input type="text" class="form-control" placeholder="Cargo">
    </div>
  </div>
  <div class="row">
    <div class="col">
      <input type="text" class="form-control" placeholder="Salario">
    </div>
    <div class="col">
      <input type="text" class="form-control" placeholder="Direccion">
    </div>
  </div>
  <div class="row">
    <div class="col">
      <input type="text" class="form-control" placeholder="Oficina">
    </div>
    <div class="col">
      <input type="text" class="form-control" placeholder="Telefono">
    </div>
  </div>
    <div class="col-sm-10">
      <button type="submit" class="btn btn-primary">Registrar</button>
    </div>
</form>
 </div>
  </div>
</template>

<script>


export default {
  name: 'Home',
  components: {
  }
}



</script>
