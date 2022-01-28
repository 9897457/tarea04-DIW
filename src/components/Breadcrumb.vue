<template>
  <section id="breadcrumb">
    <a id="inicio" href="#">Inicio</a> <p>></p>
    <a href="#">Ordenadores</a> <p>></p>
    <a id="actual" href="#">Ordenador portátil</a> 
  </section>
</template>

<script>
export default {

}
</script>

<style scoped>
  #breadcrumb {
    display:flex;
    margin-top: 2rem;
    margin-bottom: 0;
    color: #1abc9c;
  }

  #breadcrumb a{
    text-decoration: none;
    font-size: 1.2rem;
    margin-right: 0.5rem;
    margin-left: 0.5rem;
    padding: 1rem;
    color: #1abc9c;
  }

  #breadcrumb p {
    padding: 0.1rem;
  }

  #breadcrumb a:hover {
    text-decoration: none;
    color: #439184;
  }

  #breadcrumb a:active {
    text-decoration: none;
    background-color: black;
    color: white;
  }
  #actual {
    font-weight: 700;

  }

</style>