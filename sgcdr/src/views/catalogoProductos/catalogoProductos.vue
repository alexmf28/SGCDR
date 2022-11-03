<template>
    <div class="row">
        <div class="col  bg-secondary ">
            <h5 class="display-4 text-left m-4 text-white">Almacén</h5>
        </div>
        <div class="d-flex col-12 mt-3">
            <div class="col-3">
                <form class="form-inline my-2 my-lg-0">
                    <input class="form-control mr-sm-5" type="search" placeholder="Search" aria-label="Search">
                    <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Search</button>
                </form>
                <div class="m-3 text-left">
                    <h6 class="text-dark">Categorias</h6>
                    <a class="dropdown-item btn btn-light" href="#">Periféricos</a>
                    <a class="dropdown-item btn btn-light" href="#">Laptops</a>
                    <a class="dropdown-item btn btn-light" href="#">Almacenamiento</a>
                    <a class="dropdown-item btn btn-light" href="#">Monitores</a>
                </div>
            </div>
            <productosalmacen>

            </productosalmacen>

        </div>

    </div>

</template>
<script>
import axios from 'axios';
import productosalmacen from '../../components/Productos-almacen/productos-almacen.vue'
export default {
    name: 'catalogoProductos',
    components: { productosalmacen },
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