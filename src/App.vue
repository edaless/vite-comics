
<!-- 
Create un nuovo progetto utilizzando Vite e Vue 3 
e definite i componenti necessari per strutturare il layout come da screenshot allegato.
Quando la struttura a macroblocchi è pronta, 
popolate le voci di menu dinamicamente usando i data del componente.
Per oggi diamo priorità alla struttura: quando è tutto bello solido, 
passiamo al Sass (cioè la definizione dei dettagli del layout sempre tramite Sass)!
Bonus:
Creare un componente aggiuntivo per gestire la fascia azzurra con le icone.
 -->






<script setup>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'
import Card from './components/Card.vue'
</script>

<template>
  <div id="container">
    <Header />
    <Main />
    <Footer />


  </div>

</template>







<style lang="scss" scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;

}



#container {

  width: 100%;
  display: flex;
  flex-direction: column;

  // debug

  // background-color: yellow;
}
</style>


