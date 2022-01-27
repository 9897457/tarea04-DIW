<template>
  <section id="imagenes">
      <div id="imgGrande"> 
          <img v-bind:src="fotos[0]" alt="Portátil Huawei MateBoot X" copyright="cc-by portatil-img-big">
      </div>
        <div id="imgPequenya">
          <a @click="cambiarFoto(1)"><img v-bind:src="fotos[1]" alt="Portátil Huawei MateBoot X" copyright="cc-by portatil-img-small1"></a>
          <a @click="cambiarFoto(2)"><img v-bind:src="fotos[2]" alt="Portátil Huawei MateBoot X" copyright="cc-by portatil-img-small2"></a>
          <a @click="cambiarFoto(3)"><img v-bind:src="fotos[3]" alt="Portátil Huawei MateBoot X" copyright="cc-by portatil-img-small3"></a>
          <a @click="cambiarFoto(4)"><img v-bind:src="fotos[4]" alt="Portátil Huawei MateBoot X" copyright="cc-by portatil-img-small4"></a>
        </div>
      </section>    
</template>

<script>
export default {
    Name: 'ProductoImagen',
    data () {
        return {
            fotos: [
                require ('../assets/e1.jpg'),
                require ('../assets/e1.jpg'),
                require ('../assets/e2.jpg'),
                require ('../assets/e3.jpg'),
                require ('../assets/e4.jpg')]
        }
    },
    methods: {
        cambiarFoto(id) {
            this.fotos[0] = this.fotos[id]
        }
    }

}
</script>

<style scoped>
  #imagenes {
    display: flex;
    border-radius: 25px;
    padding:  0 1rem 1rem 1rem;
    margin: 1rem;
    flex-direction: column;

  }
  #imgPequenya {
    display: flex;
    justify-content: center;

  }
  #imgPequenya img {
    width: 100px;
    border:2px solid #d8d8d8;
    margin-left: 1rem;
    cursor: pointer;
  }
</style>