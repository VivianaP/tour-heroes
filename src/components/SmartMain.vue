<template>
  <div class="container">
    <h1>Tour de heroes</h1>
    <br>
    <div class="row">
      <div class="col-md-7">
        <BuscadorPoder></BuscadorPoder>
        <button type="button" class="btn btn-primary" v-on:click="mostrar = true">AGREGAR HEROE</button>
        <br>
        <br>
        <HeroeMarvel></HeroeMarvel>
      </div>
      <div class="col-md-5 nuevo-heroe">
        <NuevoHeroe v-if="mostrar"></NuevoHeroe>
      </div>
    </div>
  </div>
</template>

<script>

import BuscadorPoder from './BuscadorPoder.vue'
import HeroeMarvel from './HeroeMarvel.vue'
import NuevoHeroe from './NuevoHeroe.vue'

export default {
  name: 'SmartMain',

  data: () => ({
    mostrar: false
  }),

  components: {
    BuscadorPoder,
    HeroeMarvel,
    NuevoHeroe
  },
}

</script>

<style scoped>
h1 {
  margin: 40px 0 0;
  color: darkcyan;
  text-align: left;
}

button {
  float: right;
}

.nuevo-heroe {
  padding-left: 5%;
  padding-right: 0%;
}

a {
  color: #42b983;
}
</style>
