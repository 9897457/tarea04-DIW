<template>
 <footer id="pie">
   <img id="logo" src="../assets/logo.png" alt="Logo de la empresa" copyright="cc-by logo">
   <div id="fila1">
      <a href="#"><p>Condiciones de venta</p></a>
      <p class="espacio">|</p>
      <a href="#"><p>Informaci&oacute;n legal</p></a>
      <p class="espacio">|</p>
      <a href="#"><p>Pol&iacute;tica de privacidad</p></a>
      <p class="espacio">|</p>
      <a href="#"><p>Pol&iacute;tica de cookies</p></a>
      <p class="espacio">|</p>
      <a href="#"><p>Contactar</p></a>
      <p class="espacio">|</p>
      <a href="#"><p>Trabaja con nosotros</p></a>
   </div>
   <div id="fila2">
      <p> Carolina Hern&aacute;ndez - Todos los derechos reservados <br> Versi&oacute;n: 010. Copyright © 2022  </p>
        <div id="iconos">
          <a href="#"><img src="../assets/fb.png" alt="Logo facebook" copyright="cc-by fb"></a>
          <a href="#"><img src="../assets/twitter.png" alt="Logo twitter" copyright="cc-by twitter"></a>
          <a href="#"><img src="../assets/instagram.png" alt="Logo instagram" copyright="cc-by instagram"></a>
          <a href="#"><img src="../assets/yt.png" alt="Logo youtube" copyright="cc-by yt"></a>
        </div>
      <p>Todas las marcas son propiedad de sus respectivos fabricantes. <br> Todos los impuestos incluidos </p>
   </div>
  </footer>
</template>

<script>
export default {

}
</script>

<style scoped>
  #pie {
    background-color: #1abc9c;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin-top: 5rem;
    border-top: 2px solid black;
    border-bottom: 2px solid black;
  }

  #pie p {
    display: flex;
    padding: 1rem;
    margin: 0;
    color: black;
    text-align: center;
  }

  #logo{
    padding-top: 2rem;
    margin-right: 5rem;
  }

  #fila1 {
    display: flex;
    flex-direction: row;
    padding: 1rem;
    margin-right: 4.5rem;
  }

  #fila2 {
    display: flex;
    flex-direction: row;
  }

  #fila2 p {
    color: rgb(68, 68, 68);
  }

  #iconos {
    display: flex;
    margin: 0 1rem;
    margin-left: 4rem;
    margin-right: 4rem;
  }

  #iconos img{
    height: 3rem;
    width: 3rem;
    padding: 0 1rem 2rem 1em;
    display: flex;
  }

  .espacio {
    display: flex;
    margin: 0;
    padding: 0;
    width: 0.5rem;
  }

  #pie a {
    text-decoration: none;
  }

  #pie a p:hover {
    text-decoration: none;
    color: #439184;
  }

  #pie a p:active {
    text-decoration: none;
    background-color: black;
    color: white;
  }

  .btn:hover {
    color: #439184;
  }

</style>