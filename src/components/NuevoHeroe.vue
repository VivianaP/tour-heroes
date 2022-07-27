<template>
    <div class="row" id="heroe">
        <div class="col-md-12">
            <h2>BATMAN</h2>
            <br>
        </div>
        <div class="row">
            <div class="col-md-3 etiqueta">
                <label for="id" class="form-label ">ID</label>
            </div>
            <div class="col-md-9">
                <input type="text" class="form-control" id="id" placeholder="Ingrese el ID" v-model="id">
                <br>
            </div>
        </div>
        <div class="row">
            <div class="col-md-3">
                <label for="nombre" class="form-label etiqueta">NOMBRE</label>
            </div>
            <div class="col-md-9">
                <input type="text" class="form-control" id="nombre" placeholder="Ingrese el nombre" v-model="nombre">
                <br>
            </div>
        </div>
        <div class="row">
            <div class="col-md-3">
                <label for="poderes" class="form-label etiqueta">PODERES</label>
            </div>
            <div class="col-md-9">
                <input type="text" class="form-control" id="poderes" placeholder="Ingrese los poderes"
                    v-model="poderes">
                <br>
            </div>
        </div>
        <div class="row">
            <div class="col-md-3">
                <label for="url" class="form-label etiqueta">URL FOTO</label>
            </div>
            <div class="col-md-9">
                <input type="text" class="form-control" id="url" placeholder="Ingrese el URL foto" v-model="url">
                <br>
            </div>
        </div>
        <div class="row">
            <button type="button" class="btn btn-primary" v-on:click="agregar">GUARDAR</button>
        </div>
    </div>
</template>

<script>

export default {
    name: 'NuevoHeroe',

    data: () => ({
        id: '',
        nombre: '',
        poderes: '',
        url: ''
    }),

    methods: {
        agregar: function () {
            alert("ADD")
        }
    }

}

</script>


<style scoped>
.etiqueta {
    text-align: end;
}
</style>