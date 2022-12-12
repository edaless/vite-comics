
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
// import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <div id="container">
    <header>

    </header>
    <main>

    </main>
    <footer>

    </footer>
  </div>

</template>

<style lang="scss" scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Roboto', sans-serif;
}



#container {

  width: 100vw;
  height: 100vh;
  background-color: yellow;
  display: flex;
  flex-direction: column;
}

header {
  width: 100%;
  height: 10vh;
  background-color: white;
}

main {
  width: 100%;
  height: 100%;
  background-color: rgb(7, 102, 255);
}

footer {
  width: 100%;
  height: 480px;
  background-color: rgb(5, 230, 39);
}
</style>
