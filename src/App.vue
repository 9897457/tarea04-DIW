<template>
  <div id="body">
    <div id="zonaSuperior">
        <Cabecera />
        <Breadcrumb />
    </div>
    <div id="zonaMedia">
      <div id="producto">
        <Imagenes />
        <div id="datosProducto">
          <DatosMasContador />
        </div>
      </div>
        <Descripcion />
    </div>
    <Pie />
  </div>
</template>

<script>
import Cabecera from './components/Cabecera.vue'
import Breadcrumb from './components/Breadcrumb.vue'
import Imagenes from './components/Imagenes.vue'
import DatosMasContador from './components/DatosMasContador.vue'
import Descripcion from './components/Descripcion.vue'
import Pie from './components/Pie.vue'


export default {
  name: 'App',
  components: {
    Cabecera,
    Breadcrumb,
    Imagenes,
    DatosMasContador,
    Descripcion,
    Pie
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  margin-top: 1rem;
}

#body {
  display: flex;
  flex-direction: column;
  max-width: 1400px;
  margin: auto;
}

#zonaSuperior {
  display: flex;
  flex-direction: column;
}

#zonaMedia {
  display: flex;
  flex-direction: column;
}

#producto {
  display: flex;
  flex-direction: row;
}

#datosProducto {
  display: flex;
  flex-direction: column;
}


</style>
