<template>
  <section>
      <div id="menus">
        <div id="menu1">
          <img src="../assets/logo.png" alt="Logo de la empresa">
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
        <nav id="menu2">
          <ul>
            <li><a href="#">INICIO</a></li>
            <li><a href="#">ORDENADORES</a></li>
            <li><a href="#">TV</a></li>
            <li><a href="#">MÓVILES</a></li>
            <li><a href="#">TABLETS</a></li>
            <li><a href="#">MULTIMEDIA</a></li>
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
    padding-right: 1rem;
    padding-left: 1.5rem;
  }

  #menus {
    border: 2px solid #000a08;
    z-index:999;
    padding:0.7rem;
    display: flex;
    flex-direction: column;
  }

  #menus nav ul {
    display:flex;
    list-style: none;
    padding: 0;
    margin: 0rem 0.7rem;
  }

  #menus nav ul li a {
    display: flex;
    justify-content: space-between;
    text-decoration: none;
    color:#1abc9c;
    font-weight: 700;
    padding: 0.5rem 1rem;
  }

  #menus nav ul li a:hover, #boton:hover{
    background-color:black;
    text-decoration: none;
    color:white;
    font-weight: 700;
  }

  #menus form input{
    display: flex;
    flex-grow: 1;
    padding: 0.7rem 1rem;
    border: 2px solid #1abc9c;
    color: #181818;
    outline: none;
    line-height: 1rem;
    font-size: 1rem;
    
  }

  form {
    display: flex;
    padding: 1rem;
    flex-grow: 1;
  }

  #boton {
    font-size: 1rem;
    font-weight: 500;
    padding: 0.7rem 1.2rem;
    cursor: pointer;
    border: none;
    background-color: #1abc9c;

  }

  #menu1 {
    display: flex;
    flex-direction: row;
    align-items: center;
  }
</style>