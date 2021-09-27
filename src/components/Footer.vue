<template>
  <footer>
    <div class="my_footer-start">
      <div class="my_footer-wrapper">
        <div class="my_footer-columns">
          <div class="my_column">
            <h5>Dc Comics</h5>
            <ul>
              <li v-for="(link, index) in linksDc" :key="index"><a href="#">{{ link.text }}</a></li>
            </ul>
            <h5>Shop</h5>
            <ul>
              <li v-for="(link, index) in linksShop" :key="index"><a href="#">{{ link.text }}</a></li>
            </ul>
          </div>
          <div class="my_column">
            <h5>Dc</h5>
            <ul>
              <li v-for="(link, index) in linksUseful" :key="index"><a href="#">{{ link.text }}</a></li>
            </ul>
          </div>
          <div class="my_column">
            <h5>Sites</h5>
            <ul>
              <li v-for="(link,index) in linksSites" :key="index"><a href="#">{{ link.text }}</a></li>
            </ul>
          </div>
        </div>

        <div class="my_footer-img-box">
        </div>
      </div>
    </div>

    <div class="my_footer-end">
      <div class="my_footer-wrapper">

        <button class="my_btn-dark">ign-up now!</button>
        
        <div class="my_footer-socials">
          <ul>
            <li>
              <span>Follow Us</span>
              </li>
            <li>
              <a href="#">
                <img src="../assets/img/footer-facebook.png" alt="logo di Facebook">
              </a>
            </li>
            <li>
              <a href="#">
                <img src="../assets/img/footer-twitter.png" alt="logo di Twitter">
              </a>
            </li>
            <li>
              <a href="#">
                <img src="../assets/img/footer-youtube.png" alt="logo di YouTube">
              </a>
            </li>
            <li>
              <a href="#">
                <img src="../assets/img/footer-pinterest.png" alt="logo di Pinterest">
              </a>
            </li>
            <li>
              <a href="#">
                <img src="../assets/img/footer-periscope.png" alt="Periscope">
              </a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer',
  data: function() {
    return{

      index: 0,
      linksDc: [
        {
          text: "Characters",
          url: "#characters",
          current: false,
        },
        {
          text: "Comics",
          url: "#comics",
          current: false,
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
          text: "Videos",
          url: "#videos",
          current: false,
        },
        {
          text: "News",
          url: "#news",
          current: false,
        },
        
      ],
      linksShop: [
        {
          text: "Shop Dc",
          url: "#shopdc",
          current: false,
        },
        {
          text: "Shop Dc Collectibles",
          url: "#shopdccollectibles",
          current: false,
        },
      ],
      linksUseful: [
        {
          text: "Terms Of Use",
          url: "#termsofuse",
          current: false,
        },
        {
          text: "Privacy policy (New)",
          url: "#privacypolicynew",
          current: false,
        },
        {
          text: "Ad Choices",
          url: "#adchoices",
          current: false,
        },
        {
          text: "Advertising",
          url: "#advetising",
          current: false,
        },
        {
          text: "Jobs",
          url: "#jobs",
          current: false,
        },
        {
          text: "Subscription",
          url: "#subscription",
          current: false,
        },
        {
          text: "Talent Workshops",
          url: "#talentworkshops",
          current: false,
        },
        {
          text: "CPSC Certificates",
          url: "#cpsc",
          current: false,
        },
        {
          text: "Ratings",
          url: "#ratings",
          current: false,
        },
        {
          text: "Shop Help",
          url: "#shophelp",
          current: false,
        },
        {
          text: "Contact Us",
          url: "#contactus",
          current: false,
        },
      ],
      linksSites: [
        {
          text: "DC",
          url: "#dc",
          current: false,
        },
        {
          text: "MAD Magazine",
          url: "#madmagazine",
          current: false,
        },
        {
          text: "DC Kids",
          url: "#dckids",
          current: false,
        },
        {
          text: "Dc Universe",
          url: "#dcuniverse",
          current: false,
        },
        {
          text: "DC Power Visa",
          url: "#dcpowervisa",
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

.my_footer-start{
  background-image: url("../assets/img/footer-bg.jpg");
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}

.my_footer-wrapper{
  margin: 0px 250px;
  display: flex;
  justify-content: space-between;
  display: flex;
  align-items: center;

}

.my_footer-img-box{
  background-image: url("../assets/img/dc-logo-bg.png");
  background-position: center;
  background-size: 500px 500px;
  background-repeat: no-repeat;
  width: 500px;
  height: 353px;
}

.my_footer-end{
  background-color: $myGrey;
}

.my_footer-columns{
  display: flex;
  justify-content: space-evenly;
}

.my_column{
  padding-top: 30px;
  padding-bottom: 30px;
  padding-right: 30px;

  & ul{
    padding: 15px 0;
  }

  & ul li{
    margin: 0;
    padding: 0;
    list-style: none;
  }

  & h5{
    text-transform: uppercase;
    color: white;
    font-size: 1.1em;
  }

  & li a{
    color: $lighterGrey;
    font-size: 0.9em;
    text-decoration: none;

    &:hover{
      text-decoration: underline;
    }
  }
}

.my_footer-socials{
  
  padding: 15px 0px;

  & span{
    text-transform: uppercase;
    color: $borderBottomActiveColor;
    font-weight: bold;
  }
  
  & ul{
    display: flex;
    align-items: center;
    list-style: none;
  }

  & ul li{
    padding: 10px;
  }

  & ul li a img{
    height: 2em;
  }

}

.my_btn-dark{
  color: white;
  background-color: $myGrey;
  border: 2px solid $borderBottomActiveColor;
  text-transform: uppercase;
  padding: 7px;

  &:hover{
    background-color: $borderBottomActiveColor;
  }
}

</style>