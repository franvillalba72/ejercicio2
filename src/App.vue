<template>
  <Cabecera/>
  <Breadcrumb/>
  <Denominacion/>
  <div class="dos-columnas">
    <Imagenes/>
    <Descripcion/>
  </div>
  <Piepagina/>
</template>

<script>
import Cabecera from "./components/Cabecera.vue"
import Breadcrumb from "./components/Breadcrumb.vue"
import Denominacion from "./components/Denominacion.vue"
import Imagenes from "./components/Imagenes.vue"
import Descripcion from "./components/Descripcion.vue"
import Piepagina from "./components/Piepagina.vue"


export default {
  name: 'App',
  components: {
    Cabecera,
    Breadcrumb,
    Denominacion,
    Imagenes,
    Descripcion,
    Piepagina
  }
}
</script>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Material+Icons');

    #app {
      font-family: Avenir, Helvetica, Arial, sans-serif;
      -webkit-font-smoothing: antialiased;
      -moz-osx-font-smoothing: grayscale;
      color: #2c3e50;
      margin-top: 60px;
    }

    .boton {
        padding:0.5em 1em;
        margin: 0 1em 0 1em;
        border-radius: 0.5em;
        background-color: rgb(250, 180, 0);
        color: rgb(41,120,128);
        font-size: 1.1em;
        font-weight: bold;
        text-align: center;
        display: flex;
        align-items: center;
    }

    .boton-alterno {
        color: rgb(250, 180, 0);
        background-color: rgb(41,120,128);
    }

    a {
      text-decoration: none;
    }

    .dos-columnas {
      display: flex;
    }
</style>
