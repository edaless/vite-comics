<script>



</script>

<template>
  <div id="cont">
    <div class="larghezza">

      <div class="up">
        <!-- jumbotron -->
        <img src="../../public/img/jumbotron.jpg" alt="jumbotron">
      </div>

      <div class="middle">

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

.larghezza {
  background-color: aqua;
}

.up {
  height: 275px;
  overflow: hidden;


  img {
    width: 100%;
    height: auto;
  }
}

.middle {
  height: calc(100% / 3);
  background-color: rgb(0, 255, 115);
}

.down {
  height: calc(100% / 3);
  background-color: rgb(212, 255, 0);
}
</style>
