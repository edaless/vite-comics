<script>

export default {

  data() {
    return {
      links: [
        {
          text: "characters",
          path: "#"

        },
        {
          text: "comics",
          path: "#"

        },
        {
          text: "movies",
          path: "#"

        },
        {
          text: "tv",
          path: "#"

        },
        {
          text: "games",
          path: "#"

        },
        {
          text: "collectibles",
          path: "#"

        },
        {
          text: "videos",
          path: "#"

        },
        {
          text: "fans",
          path: "#"

        },
        {
          text: "news",
          path: "#"

        },
        {
          text: "shop",
          path: "#"

        }
      ],
      activeLink: 0
    }
  },
  methods: {
    aggiornoActiveLink(index) {
      this.activeLink = index;
    }

  }
}
</script>

<template>
  <div id="cont">
    <div class="larghezza">

      <div class="logo">
        <img src="../../public/img/dc-logo.png" alt="">
      </div>

      <div id="links">
        <div class="link" v-for="(link, index) in links" :class="{ active: activeLink === index }" :key="index"
          @click="aggiornoActiveLink(index)">
          {{ (link.text).toUpperCase() }}
        </div>
      </div>

    </div>
  </div>
</template>

<style lang="scss" scoped>
$colorheader : white;


#cont {
  position: fixed;
  display: flex;
  justify-content: center;
  width: 100%;
  height: var(--h-header);
  background-color: $colorheader;
}

.logo {
  height: 100%;
  padding: 0 5px;
  display: flex;
  align-items: center;
}

img {
  width: auto;
  height: 75%;
}

.larghezza {
  display: flex;
  justify-content: space-between;
}

#links {
  display: flex;
  justify-content: center;
  align-items: center;
}

.link {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100%;
  // width: 40px;
  font-size: 12px;
  font-weight: 900;
  margin-left: 15px;
  color: #4f4f4f;



  &:hover {
    color: var(--color-blue);
    border-bottom: 4px solid var(--color-blue);
    // per non far muovere la scritta:
    border-top: 4px solid $colorheader;
  }
}

.active {
  color: var(--color-blue);
  border-bottom: 4px solid var(--color-blue);
  // per non far muovere la scritta:
  border-top: 4px solid $colorheader;

}
</style>
