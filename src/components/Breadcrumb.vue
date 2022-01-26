<template>
  <section id="breadcrumb">
      <a id="inicio" href="#">Inicio</a>>
      <a href="#">Ordenadores</a>>
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

  #breadcrumb a, 
  #breadcrumb a:hover, 
  #breadcrumb a:visited{
    text-decoration: none;
    font-size: 1.2rem;
    margin-right: 0.5rem;
    margin-left: 0.5rem;
    color: #1abc9c;
}

#actual {
    font-weight: 700;

}

</style>