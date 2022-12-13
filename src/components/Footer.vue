<script>

export default {

  data() {
    return {
      colonne: [
        {
          titolo: "dc comics",
          elementi: [
            "Characters",
            "Comics",
            "Movies",
            "TV",
            "Games",
            "Videos",
            "News"

          ]
        },
        {
          titolo: "shop",
          elementi: [
            "Shop DC",
            "Shop DC Collectibles"


          ]
        },
        {
          titolo: "dc",
          elementi: [
            "Terms Of Use",
            "Privacy Policy (New)",
            "Ad Choices",
            "Advertising",
            "Jobs",
            "Subscriptions",
            "Talent Workshops",
            "CPSC Certificates",
            "Ratings",
            "Shop Help",
            "Contact Us"
          ]
        },
        {
          titolo: "sites",
          elementi: [
            "DC",
            "MAD Magazine",
            "DC Kids",
            "DC Universe",
            "DC Power Visa"
          ]
        }
      ]
    }
  },
  methods: {


  }
}



</script>

<template>
  <div id="cont">
    <div id="prima-meta">
      <div class="larghezza">
        <div class="sinistra">
          <div class="colonna" v-for="colonna in colonne">
            <strong>
              {{ colonna.titolo.toLocaleUpperCase() }}
            </strong>
            <div v-for="elemento in colonna.elementi">
              {{ elemento }}
            </div>


          </div>
        </div>
        <div class="destra">
          <img src="../../public/img/dc-logo-bg.png" alt="">
        </div>

      </div>
    </div>
    <div id="seconda-meta">
      <div class="larghezza">
        <div class="button">SIGN-UP NOW!</div>
        <div class="dflex">
          <div id="follow">FOLLOW US</div>
          <div class="social">
            <img src="../../public/img/footer-facebook.png" alt="">
          </div>
          <div class="social">
            <img src="../../public/img/footer-twitter.png" alt="">
          </div>
          <div class="social">
            <img src="../../public/img/footer-youtube.png" alt="">
          </div>
          <div class="social">
            <img src="../../public/img/footer-pinterest.png" alt="">
          </div>
          <div class="social">
            <img src="../../public/img/footer-periscope.png" alt="">
          </div>
        </div>

      </div>
    </div>
  </div>
</template>






<style lang="scss" scoped>
#cont {
  display: flex;
  align-items: center;
  flex-direction: column;
  width: 100%;
  // height: 480px;
  background-color: #333333;
}

#prima-meta {
  display: flex;
  justify-content: center;
  height: 350px;
  width: 100%;
  // padding: 10px;
  background-image: url("../../public/img/footer-bg.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}

#seconda-meta {
  display: flex;
  justify-content: center;
  height: 110px;
  width: 100%;

  // padding: 10px;
  .larghezza {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

}

.sinistra {
  display: flex;
  flex-direction: column;
  flex-wrap: wrap;
  padding: 20px 0;
}

.destra {
  display: flex;
  justify-content: center;
  align-items: center;
  overflow-y: hidden;

  img {

    width: 530px;
  }
}

.larghezza {
  display: flex;
  justify-content: space-between;


  // debug
  // background-color: rgb(132, 255, 0);
}

.colonna {
  display: flex;
  flex-direction: column;
  margin-top: 10px;
  width: 150px;


  // debug
  // background-color: aqua;
  strong {
    margin-bottom: 20px;
    font-size: 20px;
    color: white;
  }

  div {
    margin-bottom: 5px;
    font-size: 13px;
    color: #848584;

    &:hover {
      color: white;
    }
  }
}

.button {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 145px;
  height: 50px;
  font-weight: 700;
  color: white;
  // background-color: aqua;
  border: 2px solid var(--color-blue);
}

.dflex {
  display: flex;
  align-items: center;
  justify-content: end;


}

#follow {
  font-weight: 700;
  font-size: 20px;
  margin-right: 5px;
  color: var(--color-blue);
}

.social {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 30px;
  height: 30px;
  margin-left: 20px;

  img {
    width: 100%;
    height: 100%;
  }

}
</style>
