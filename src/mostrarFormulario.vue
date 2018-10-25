<template>
    <form action="" class="form">
      <!-- <h3>{{titulo}}</h3> -->
      <!-- Slot me permite mostrar todo lo que esta dentro de la etiqueta mostrarFormulario -->
      <!-- Algo asi como el yield de laravel  -->
      <slot></slot>
      <!-- <div class="form-group">
        <label for="correo">Correo Electrónico</label>
        <input type="email" class="form-control"
          id="correo" placeholder="Escribe tu correo electronico">
      </div>
      <div class="form-group">
        <label for="clave">Contraseña</label>
        <input type="password" class="form-control"
          id="clave" placeholder="Escribe tu Contraseña">
      </div>
      <button class="btn btn-primary">Iniciar Sesión</button> -->
    </form>
</template>
<script>
  export default {
    // props: ['titulo']
  }
</script>
<style>

</style>

