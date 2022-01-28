<template>
  <section>
      <div id="menus">
        <div id="menu1">
          <img src="../assets/logo.png" alt="Logo de la empresa" copyright="cc-by logo">
          <form @submit.prevent="handleEnviar">
            <input type="search" v-model="buscar" placeholder="Buscar productos ...">
            <button id="boton">Buscar</button>
          </form>
          <nav>
            <ul id="lista1">
              <li id="espacio">&nbsp;</li>
              <li>|</li>
              <li><a href="#">REGISTRO</a></li>
              <li>|</li>
              <li><a href="#">INICIAR SESIÓN</a></li>
              <li>|</li>
            </ul>
          </nav>
        </div>
        <nav id="menu2">
          <ul id="lista2">
            <li><a href="#">INICIO</a></li>
            <li>|</li>
            <li><a href="#">ORDENADORES</a></li>
            <li>|</li>
            <li><a href="#">TV</a></li>
            <li>|</li>
            <li><a href="#">MÓVILES</a></li>
            <li>|</li>
            <li><a href="#">TABLETS</a></li>
            <li>|</li>
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
    border-bottom: 2px solid black;
    z-index:999;
    display: flex;
    flex-direction: column;
  }

  #menus nav ul {
    display:flex;
    list-style: none;
    padding: 0;
    margin: 0rem 0.7rem;
  }

  
  #menus #menu1 ul li a {
    display: flex;
    text-decoration: none;
    color:black;
    font-weight: 700;
    padding: 1rem 1.5rem;
  }

  #menus #menu2 ul li a {
    display: flex;
    text-decoration: none;
    color:black;
    font-weight: 700;
    padding: 1rem;
    padding-left: 7.1rem;
    padding-right: 7.1rem;
  }

  #menus #menu1 ul li a:hover, 
  #menus #menu2 ul li a:hover,
  #boton:hover{
    text-decoration: none;
    color: #439184;
    font-weight: 700;
  }

  #menus #menu1 ul li a:active, 
  #menus #menu2 ul li a:active,
  #boton:active{
    background-color: black;
    color: white;
    text-decoration: none;
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
    font-weight: 700;
  }

  #menu1 {
    display: flex;
    flex-direction: row;
    align-items: center;
  }

  #menu2 {
    border-top: 2px solid black;
    background-color: #1abc9c;
  }

  #lista1{
    display: flex;
    justify-content: space-around;
    align-items: center;
  }


  #lista2{
    display: flex;
    justify-content: space-around;
    align-items: center;
    flex-grow: 1;
  }

  #espacio {
    display: flex;
    padding-right: 1rem;
  }
  
</style>