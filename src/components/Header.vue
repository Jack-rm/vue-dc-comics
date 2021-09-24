<template>
  <div>
    <header>
      <img src="../assets/img/dc-logo.png" alt="Logo Dc Comics">
      <nav>
        <ul>
          <li v-for="(link, index) in links" :key="index" :class="{ active : link.current }">
            <a href="#">{{ link.text }}</a>
          </li>
        </ul>
      </nav>
    </header>
  </div>
</template>

<script>
export default {
  name: 'Header',
  data: function () {
    return{

      index: 0,
      links: [
        {
          text: "Characters",
          url: "#characters",
          current: false,
        },
                {
          text: "Comics",
          url: "#comics",
          current: true,
        },
                {
          text: "Movies",
          url: "#movies",
          current: false,
        },
                {
          text: "Tv",
          url: "#tv",
          current: false,
        },
                {
          text: "Games",
          url: "#games",
          current: false,
        },
                {
          text: "Collectibles",
          url: "#collectibles",
          current: false,
        },
                {
          text: "Videos",
          url: "#videos",
          current: false,
        },
                {
          text: "Fans",
          url: "#fans",
          current: false,
        },
                {
          text: "News",
          url: "#news",
          current: false,
        },
                {
          text: "Shop",
          url: "#shop",
          current: false,
        },
      ],
    }
  },

}
</script>

<style lang="scss">
@import "../style/variables.scss";
@import "../style/general.scss";

header {
  margin: 0px 250px;
  
  text-align: center;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

img {
  height: 100px;
}

ul{
  display: flex;
  list-style: none;
}

ul li{
  padding-top: 65px;
  padding-bottom: 65px;
  margin-left: 40px;
  border-bottom: 6px solid transparent;

  &.active:hover{
  border-bottom: 6px solid $borderBottomActiveColor;
  }
}

li a{
  color: $darkerGrey;
  text-decoration: none;
  text-transform: uppercase;
}

</style>