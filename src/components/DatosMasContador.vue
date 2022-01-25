<template>
  <section id="datosMasContador">
      <h1>Portátil Huawei MateBook X</h1>
      <div id="precio">
        <h2>750,69€</h2> <p id="iva1">SIN IVA: <br>620,41€</p>
      </div>
      <div id="informacion">
        <div id="titulos">
          <p>Envío: </p>
          <p>Marca: </p>
          <p>Cantidad: </p>
          <p>Env&iacute;o a domicilio: </p>
        </div>
        <div id="descripcion">
          <span id="envio"> ¡¡ENV&Iacute;O GRATIS!!</span> 
          <span id="marca"> <a href="#">HUAWEI</a> - P/N: 53019689 | Cod. Art&iacute;culo: 254954</span>
          <div id="cantidad">
            <button class="btn" @click="cambiarContador('-1')" type="button" name="btn">-</button>
            <input id="cantidadInput" type="text" name="name" :value="contador">
            <button class="btn" @click="cambiarContador('1')" type="button" name="btn">+</button>
          </div>
          <span id="envioDomicilio">¡En stock! ¡Rec&iacute;belo el jueves 27 de enero!</span>
        </div>
           
      </div>
      <br>
      <button id="btnCompra"><span class="material-icons">shopping_cart</span> AÑADIR CARRITO</button>
  </section>
</template>

<script>
export default {
  Name: 'ProductoDatos',
    data () {
        return {
            contador: 1
        }
    },
    methods: {
        cambiarContador(num) {
            this.contador += +num;
            if (!isNaN(this.contador) && (this.contador < 0)) {
              this.contador = 0
            }
        }
    }


}

</script>

<style scoped>

#datosMasContador {
  margin-top: 5rem;
}

h1 {
  display: flex;
  font-size: 2.2rem;
  margin: 2rem 0 0 0;
  padding: 0;
}

h2 {
  font-size:3rem;
  color: #1abc9c;
  margin: 0;
  padding: 0;
}

#precio {
  display: flex;
  flex-direction: row;
}

#iva1 {
  display: flex;
  align-items: center;
  margin: 0;
  padding-bottom: 0.5rem;
  padding-left: 1rem;
  color: gray;
}

#informacion {
  display: flex;
  flex-direction: row;
}

#datosMasContador #informacion p,
#datosMasContador #informacion span {
  display: flex;
  padding: 0.5rem 0 0.5rem 0;
  margin: 0.5rem 0 0.5rem 0;
}

#marca {
  font-size: 0.9rem;  
}

#titulos {
  margin-right: 1rem;
}

#cantidadInput {
  border: none;
  text-align: center;
  width: 2rem;
  font-size: 1rem;
}
.btn {
  border: 1px solid #d8d8d8;
  width: 2rem;
  height: 2rem;
}

button:focus, input:focus {
  outline: 0;
}

#envio {
  color: #1abc9c;
}

#envioDomicilio {
  background-color: #1abc9c;
  color: white;
}

#btnCompra {
  display: flex;
  justify-content: space-between;
  align-items: center;
  border: 1px solid #d8d8d8;
  padding: 1.3rem;
  width: 12rem;
  height: 3rem;
}

#cantidad {
  display: flex;
  align-items: center;
}
#datosMasContador #informacion #descripcion a {
  text-decoration: none;
  color:#1abc9c;
  font-weight: 700;
  padding-right: 0.5rem;
}
  
</style>