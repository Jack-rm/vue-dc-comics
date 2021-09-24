<template>
  <div>
    <main>
     
     <section class="my_content-section">
        <div class="my_content">
          <h3> --- Content goes here --- </h3>
        </div>
      </section>
      
      <section class="my_features-section">
        <div class="my_features">
          <h3> --- Features go here --- </h3>
        </div>
      </section>

    </main>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
@import "../style/variables.scss";
@import "../style/general.scss";

main .my_content-section{
  background-color: $darkerGrey;
  padding: 50px 0px;
}

main .my_features-section{
  background-color: $borderBottomActiveColor;
  padding: 50px 0px;
}

.my_content{
    padding: 0px 250px;
    color: white;
}

.my_features{
    margin: 0px 250px;
    color: white;
}

</style>