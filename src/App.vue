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
        <keep-alive>
          <component v-bind:is="componenteSelecionado"></component>
        </keep-alive>

    </div>
  </div>
</template>

<script>
// la etiqueta keep-alive es reservado par Vue y no podemos suarlo para mas nada.
// si usamos keep alive, no podemo usar el ciclo de vida destroyed(),  estos si se puede
// usar activated(), deactivated()

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
