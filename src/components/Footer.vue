<template>
  <footer>
    <div class="my_footer-start">
      <div class="my_footer-wrapper">
        <div>
          <p>colonna</p>
        </div>
        <div>
          <p>colonna</p>
        </div>
        <div>
          <p>colonna</p>
        </div>

        <div>
          <img src="" alt="Big logo Dc Comics">
        </div>
      </div>
    </div>

    <div class="my_footer-end">
      <div class="my_footer-wrapper">

        <button>bottone</button>
        
        <div>
          <p>Follow us</p>
          <p>facebook</p>
          <p>twitter</p>
          <p>yt</p>
          <p>pinterest</p>
          <p>localizzazione</p>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {

}
</script>

<style lang="scss">
@import "../style/variables.scss";
@import "../style/general.scss";

.my_footer-start{
  background-image: url("../assets/img/footer-bg.jpg");
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}

.my_footer-wrapper{
    margin: 0px 250px;
}

.my_footer-end{
  background-color: $myGrey;
}
</style>