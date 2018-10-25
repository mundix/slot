<template>
  <div class="container">
    <div class="jumbotron">
      <!-- <mostrarFormulario titulo="Cambiar Contraseña"></mostrarFormulario> -->
        <!-- Quiero pasar el titulo de esta forma usando slot  -->
      <mostrarFormulario>
        <h3>Cambiar Contrasenña</h3>
        <div>
          <div class="form-group">
            <label for="correo">Correo Electrónico</label>
            <input type="email" class="form-control"
              id="correo" placeholder="Escribe tu correo electronico">
          </div>
          <div class="form-group">
            <label for="clave">Contraseña</label>
            <input type="password" class="form-control"
              id="clave" placeholder="Escribe tu Contraseña">
          </div>
          <button class="btn btn-primary">Iniciar Sesión</button>
        </div>
      </mostrarFormulario>
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
