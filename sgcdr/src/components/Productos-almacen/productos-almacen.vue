<template>                 
            <div class="container">
                <div class="row">
                   
                    <div class="col-sm"
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
                        <div>
                            <button type="button" class="btn btn-outline-info">Agregar</button>
                            <button type="button" class="btn btn-outline-info">Agregar</button>
                            <button type="button" class="btn btn-outline-info">Agregar</button>
                        </div>
                    </div>
                </div>
            </div>
</template>
<script>
import axios from 'axios';
import agregar from '';
export default {
    name: 'productos-almacen',
    data() {
        return {
            users: null,
        };
    },
    created: function () {
        axios
            .get('https://jsonplaceholder.typicode.com/users')
            .then(res => {
                this.users = res.data;
            })
    }
}
</script>
<style>
.logo{
  width:50%;

}
</style>