<template>
  <div>
    <main>
     
     <section class="my_jumbotron">
      <div class="my_title-marker">
        <h2>Current Series</h2>
      </div>
     </section>
     <section class="my_content-section">
        <div class="my_content">
          <Box v-for="(comic, index) in comics" :key="index" :title="comic.series" :source="comic.thumb" />
        </div>
        <button class="my_btn-light">Load More</button>
      </section>

    </main>
  </div>
</template>

<script>
import Box from './Box.vue';
import comics from '../data/comics.js';

export default {
  name: "Main",
  components: {
      Box,
  },
  data: function() {
    return {
      comics,
    }
  }

}
</script>

<style lang="scss">
@import "../style/variables.scss";
@import "../style/general.scss";

.my_jumbotron{
  position: relative;
  height: 60vh;
  width: 100%;
  background-image: url("../assets/img/jumbotron.jpg");
  background-repeat: no-repeat;
  background-size: cover;
}

.my_title-marker{
  position: absolute;
  bottom: -20px;
  left: 430px;
  background-color: $borderBottomActiveColor;
  padding: 5px 20px;
  color: white;
  text-transform: uppercase;

}

main .my_content-section{
  background-color: $darkerGrey;
  text-align: center;
}

.my_content{
  padding: 0px 450px;
  display: flex;
  flex-wrap: wrap;
}

.my_btn-light{
  color: white;
  background-color: $borderBottomActiveColor;
  border: 2px solid $darkerGrey;
  font-weight: bold;
  text-transform: uppercase;
  padding:10px 60px;
  margin: 20px 0px;

  &:hover{
    background-color: $myGrey;
  }
}

</style>