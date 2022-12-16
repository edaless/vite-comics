<script>
import Card from './Card.vue';



</script>

<template>
  <div id="cont">
    <div class="larghezza">

      <div class="up">
        <!-- jumbotron -->
        <img src="../../public/img/jumbotron.jpg" alt="jumbotron">
      </div>

      <div class="middle">
        <div class="larghezza">
          dddd

          <Card />
          <Card />
        </div>

      </div>

      <div class="down">

      </div>

    </div>
  </div>
</template>

<style lang="scss" scoped>
#cont {
  margin-top: var(--h-header);
  display: flex;
  justify-content: center;
  width: 100%;
  height: 900px;
  background-color: #212121;

}


.up {
  height: 275px;
  overflow: hidden;
  display: flex;
  justify-content: center;


  img {
    width: auto;
    height: 250%;
  }
}

.middle {
  height: 500px;
  background-color: #212121;
}

.down {
  height: calc(100% / 3);
  background-color: rgb(212, 255, 0);
}
</style>
