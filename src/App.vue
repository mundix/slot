<template>
  <div class="container">
    <div class="jumbotron">
      <button class="btn btn-primary"
        @click="componenteSelecionado='iniciarSesion'">
          Iniciar Sesion
        </button>
      <button class="btn btn-primary"
        @click="componenteSelecionado='cambiarClave'">
          Cambiar Clave
        </button>
        <component v-bind:is="componenteSelecionado"></component>
    </div>
  </div>
</template>

<script>

import MostrarFormulario from './mostrarFormulario.vue';
import IniciarSesion from './IniciarSesion.vue';
import CambiarClave from './CambiarClave.vue';

export default {
  components: {
    mostrarFormulario: MostrarFormulario,
    iniciarSesion: IniciarSesion,
    cambiarClave: CambiarClave
  },
  data(){
    return {
      componenteSelecionado: 'iniciarSesion'
    }
  }
}
</script>

<style scoped>

</style>
