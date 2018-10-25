<template>
  <div class="container">
    <div class="jumbotron">
      <mostrarFormulario></mostrarFormulario>
    </div>
  </div>
</template>

<script>
// Vamos a crear un componente que tenga varios formularioo uno
import MostrarFormulario from './mostrarFormulario';
export default {
  components: {
    mostrarFormulario: MostrarFormulario
  },
  data(){

  }
}
</script>

<style>

</style>
