<template>
  <div class="home">
    <div class="margin-container"></div>
    <div>
      <h1>Bienvenid@ a Open COVID-19 Test</h1>
      <p class="home-p">
        Un test de autoevaluación para el COVID-19 de código abierto que
        devuelve los mismos resultados que
        <a href="https://www.coronamadrid.com/">coronamadrid.com</a> pero no
        almacena tus valiosos datos.
      </p>
      <p class="home-p">
        También puedes entrar al
        <a href="https://github.com/celiavelmar/open-covid19-test"
          >repositorio en Github de celiavelmar
          <font-awesome-icon :icon="['fab', 'github']"></font-awesome-icon
        ></a>
        para conocer el algoritmo que usa dicha aplicación (y también
        esta) y cómo lo ha descubierto o como hizo para ver el código fuente.
      </p>
       <p class="home-p">
        También puedes entrar a 
        <a href="https://github.com/ccardozom/"
          >mi repositorio en Github
          <font-awesome-icon :icon="['fab', 'github']"></font-awesome-icon
        ></a>
        para ver el algoritmo modificado.
      </p>
      <info-panel
        class="home-info-panel"
        text="La información obtenida a través del uso de esta aplicación no sustituye
        ni pretende sustituir, en ningún caso, el consejo de un profesional
        médico. Si crees que tienes síntomas compatibles con el COVID-19 ponte
        en contacto con el teléfono del 
        <a href="https://www.mspbs.gov.py/covid-19.php?q=CORONAVIRUS&modo=1"
          >centro nacional de enlace 154.
          <font-awesome-icon :icon="['fab', 'github']"></font-awesome-icon
        ></a>"
      ></info-panel>
      <div class="center">
        <router-link to="/test">
          <button>¡Entendido(Taupéicha)! Hacer Test(Jajapo Kuaara'ã)</button>
        </router-link>
      </div>
    </div>
    <div class="margin-container"></div>
  </div>
</template>

<script>
import InfoPanel from '@/components/InfoPanel.vue';

export default {
  name: 'Home',
  components: {
    InfoPanel
  }
};
</script>

<style>
a {
  color: cornflowerblue;
}

.home {
  padding-top: 30px;
  display: flex;
  flex-direction: row;
}

.home-p {
  padding: 1% 5%;
}

.home-info-panel {
  margin: 1% 5%;
}

.margin-container {
  display: flex;
  width: 20%;
}
</style>
