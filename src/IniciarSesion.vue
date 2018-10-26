<template>
  <div class="container">
    <div class="jumbotron">
      <!-- <mostrarFormulario titulo="Cambiar Contraseña"></mostrarFormulario> -->
        <!-- Quiero pasar el titulo de esta forma usando slot  -->
      <mostrarFormulario>
        <div slot="titulo">
          <h3>Iniciar Sesion</h3>
        </div>
        <div slot="elementos">
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
        </div>
        <div slot="boton">
          <button class="btn btn-primary">Iniciar Sesion</button>
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
  data() {
    return { }
  },
  destroyed() {
    //PAra no perder la info debemos usar algo keepalive
    console.log("El componente fue destruido");
  },
  activated(){
    console.log("Activado");
  },
  deactivated(){
    console.log("Fue desacticado");
  }
}
</script>

<style scoped>

</style>
