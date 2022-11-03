<template>                 
            <div class="container">
                <div class="row">
                   
                    <div class="col-sm my-4"
                    v-for="n in 12"
                    :v-key="n">
                       <div 
                       image="../../assets/Logo-Rayotec.png"
                       name="Product"
                       :price="300"></div> 
                        <img src="../../assets/Logo-Rayotec.png" alt="">
                        <div>
                            <p><small>MSI</small></p>
                            <p>Laptop Gamer MSI GL65 15.6" 16GB RAM 512GB SSD</p>
                            <p><strong>S/ 7,390 un</strong></p>
                        </div> 
                        <div class="d-flex">
                            <button v-if="contador < 1" v-on:click="contador = contador + 1" type="button" class="btn btn-outline-info">Agregar</button>
                            <button v-if="contador > 0" v-on:click="contador = contador - 1" type="button" class="btn btn-outline-info"><i class="fa-solid fa-minus"></i></button>
                            <p v-if="contador > 0">{{contador}}</p>
                            <button v-if="contador > 0" v-on:click="contador = contador + 1" type="button" class="btn btn-outline-info"><i class="fa-solid fa-plus"></i></button>
                        </div>
                    </div>
                </div>
            </div>
</template>
<script>
import axios from 'axios';

export default {
    name: 'productos-almacen',
    data() {
        return {
            users: null,
            contador: 0
           
        };        
       
    },
    created: function () {
        axios
            .get('https://jsonplaceholder.typicode.com/users')
            .then(res => {
                this.users = res.data;
            })
    },
    ocultarAgregar(){
        if(contador += 1){

        }
    }
}
</script>
<style>
.logo{
  width:50%;

}
</style>