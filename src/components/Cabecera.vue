<template>
  <section>
      <img src="../assets/logo.png" alt="Logo de la empresa">
      <div id="menu">
        <nav>
          <ul>
            <li><a href="#">INICIO</a></li>
            <li><a href="#">ORDENADORES</a></li>
            <li><a href="#">TV</a></li>
            <li><a href="#">MÓVILES</a></li>
            <li><a href="#">TABLETS</a></li>
            <li><a href="#">MULTIMEDIA</a></li>
          </ul>
        </nav>
        <form @submit.prevent="handleEnviar">
          <input type="text" v-model="buscar" placeholder="Buscar productos ...">
          <button id="boton">Buscar</button>
        </form>
        <nav>
          <ul>
            <li><a href="#">REGISTRO</a></li>
            <li><a href="#">INICIAR SESIÓN</a></li>
          </ul>
        </nav>
      </div>
  </section>
</template>

<script>
export default {
  name: 'Cabecera',
  data() {
    return {
      buscar: "",
    }
  },
  methods: {
    handleEnviar() {
      console.log("Busqueda enviada. Se ha introducido: "+this.buscar);
      this.buscar = '';
        
    }
  }
}
</script>

<style scoped>
  section img {
    display: flex;
    padding-bottom: 1rem;
  }

  #menu {
    background: #1abc9c;
    z-index:999;
    padding:0.7rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  #menu nav ul {
    display:flex;
    list-style: none;
    padding: 0;
    margin: 0rem 0.7rem;
  }

  #menu nav ul li a {
    display: flex;
    justify-content: space-between;
    text-decoration: none;
    color:white;
    font-weight: 700;
    padding: 0.5rem 1rem;
  }

  #menu nav ul li a:hover, #boton:hover{
    background-color:black;
    text-decoration: none;
    color:white;
    font-weight: 700;
  }

  #menu form input{
    padding: 0.7rem 1rem;
    border-style: solid;
    border: 2px solid #1abc9c;
    color: #181818;
    outline: none;
    line-height: 1rem;
    font-size: 1rem;
  }

  #boton {
    font-size: 1rem;
    font-weight: 500;
    padding: 0.7rem 1.2rem;
    cursor: pointer;
    border: none;
    background-color: #1abc9c;

  }
</style>