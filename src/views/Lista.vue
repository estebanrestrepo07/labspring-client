<template>
    <div class="container">
        <div class="row">
                <div class="col-xl-12 ">
                    <h1 class="text-center">Lista de empleados</h1>
                    <table class="table table-striped text-center">
                        <thead class="thead-dark">
                        <tr>
                            <th class="text-center">Documento de identidad</th>
                            <th class="text-center">Nombre completo</th>
                            <th class="text-center">Genero</th>
                            <th class="text-center">Estado Civil</th>
                            <th class="text-center">Salario</th>
                            <th class="text-center">Email</th>
                            <th class="text-center">Telefono</th>
                            <th class="text-center">Eliminar</th>
                            <th class="text-center">Actualizar</th>
                        </tr>
                        </thead>
                        <tbody>
                        <tr v-for="(reg,index) in list" :key="index"> 
                            <td v-text="reg.empleadoId"></td> 
                            <td v-text="reg.nombreCompleto"></td>
                            <td v-text="reg.genero"></td>
                            <td v-text="reg.estadoCivil"></td>                             
                            <td v-text="reg.salario"></td>
                            <td v-text="reg.email"></td>
                            <td v-text="reg.telefono"></td>
                            <td >
                                <button class="btn btn-danger" @click="despedir(reg.empleadoId)">Eliminar</button>
                            </td>
                            <td>  <router-link :to="{ name: '/actualizar', params: { Emp: reg.empleadoId }}" class="btn btn-success">Actualizar</router-link>
                            </td>
                        </tr>
                        </tbody>
                    </table>
                </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "test",
        created() {
        },
        data() {
            return{
            list:[]
        }
    }
    ,
    mounted() {
        this.cargar()
        },
    
    methods: {
        despedir(index){
            fetch('https://labspring-udea.herokuapp.com/delEmp/'+index,{
                method: 'DELETE'
            }).then( () => {
                this.cargar();
            })
        },
       
        cargar(){
            fetch('https://labspring-udea.herokuapp.com/findAllEmp').
            then(res => res.json().then((data) => {
                this.list = data}));
        },
    }
    }
</script>
