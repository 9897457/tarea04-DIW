<template>
  <section id="descripcion">
    <div id="titulos">
      <a @click="change"><h4 id="titulo1">DESCRIPCI&Oacute;N DEL PRODUCTO</h4></a>
      <p class="espacio">&nbsp;</p>
      <a @click="change"><h4 class="titulo2">V&Iacute;DEO DEL PRODUCTO</h4></a>
    </div>
    <div id="txtTitulo1" v-if="click">
       <ul>
          <li>Ligero, potente, hermoso. </li>
          <li>El Huawei MateBook X con su pantalla de 13 pulgadas, sistema de sonido Dolby, 12,5 mm de espesor, 1,05 kg y sensor de huella dactilar integrado, integrarás sin esfuerzo las exigencias profesionales del trabajo y el ocio de tu vida personal. </li>
          <li>Lo suficientemente ligero como para cambiar el mundo donde quiera que estés, y cuando quiera que lo desees. Huawei MateBook X puede ser más pequeño que una lámina A4, pero el procesador de 7ª Generación de Intel® Core™ desarrolla un rendimiento prácticamente ilimitado. </li>
          <li>Con la ingeniería aeroespacial aplicada en Huawei MateBook X, tendrás tu ordenador siempre refrigerado: el sobrecalentamiento será cosa del pasado.</li>
          
          <li><br><br><b><u>Caracter&iacute;sticas:</u></b></li>
          <li><br><b>HUAWEI MateBook X es pequeño pero poderoso;</b> su procesador de hasta 7ª generación Intel® Core™ i7 proporciona potencia suficiente tanto para trabajo como para entretenimiento. </li>
          <li><b>La ingeniería aeroespacial permite al HUAWEI MateBook X permanecer frío</b> gracias a sus materiales de cambio de fase (usados en la industria espacial), lo que significa que el sobrecalentamiento es una cosa del pasado.</li>
          <li><b>El botón de encendido dos en uno del HUAWEI MateBook X y su sensor de reconocimiento por huella dactilar</b> te ayudan a arrancarlo de forma rápida y segura para funcionar a la velocidad de tu vida.</li>
          <li><b>Seguridad total.</b> Hoy en día utilizamos los dispositivos electrónicos para todo tipo de cosas; desde transacciones bancarias hasta el almacenamiento de documentos importantes. Por ello, la seguridad nunca está de más. </li>  
          <li>El portátil Huawei está equipado con un sensor de huella dactilar para que sólo tú puedas iniciar sesión y utilizarlo. </li>
          <li><b>Memoria ultrarrápida. </b>Con el disco duro de 256 GB SSD podrás arrancar tu Windows 10 como un verdadero tiro. En un abrir y cerrar de ojos tendrás listo tu portátil.  </li>
      </ul>
    </div>
    <div id="videoTitulo2" v-else>
      <video-embed src="https://www.youtube.com/watch?v=s4ObxcdXoFE"></video-embed>
    </div>
     
  </section>
</template>

<script>
export default {
  data() {
    return {
      click: false
    }
  }
  
}
</script>

<style scoped>

#descripcion {
  display: flex;
  flex-direction: column;
  justify-content: center;
  flex-wrap: wrap;
  margin: 1rem;
  margin-left: 25rem;
  margin-right: 25rem;
}
#descripcion #titulos h4 {
  display: flex;
  color: #1abc9c;
  border-bottom: 5px solid black;
  padding: 1rem;
}

#titulos {
  display: flex;
  flex-direction: row;
}

#descripcion ul{
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  list-style: none;
  padding: 0;
  line-height: 1.5rem;
}

.espacio {
  display: flex;
  width: 3rem;
}

</style>