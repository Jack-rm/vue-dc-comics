<template>
    <div>
        <section class="my_features-section">
            <div class="my_features">
                <ul>
                    <li v-for="(link,index) in links" :key="index">
                        <a href="#">
                            <img :src="link.img"/>
                            {{ link.text }}
                        </a>
                    </li>
                </ul>
            </div>
        </section>
    </div>
</template>

<script>
export default {
    name: 'Features',
    data: function() {
        return{
            index:0,
            links: [
                {
                    text: "Digital Comics",
                    img: require("../assets/img/buy-comics-digital-comics.png")
                },
                {
                    text: "DC Merchandise",
                    img: require("../assets/img/buy-comics-merchandise.png")
                },
                {
                    text: "Subscription",
                    img: require("../assets/img/buy-comics-subscriptions.png")
                },
                {
                    text: "Comic Shop Locator",
                    img: require("../assets/img/buy-comics-shop-locator.png")
                },
                {
                    text: "DC Power Visa",
                    img: require("../assets/img/buy-dc-power-visa.svg")
                },
            ],
        }
    }

}
</script>

<style lang="scss">
@import "../style/variables.scss";
@import "../style/general.scss";

.my_features-section{
  background-color: $borderBottomActiveColor;
  padding: 50px 0px;
}

.my_features{
    margin: 0px 250px;
    color: white;

    & ul{
        display: flex;
        align-items: center;
        justify-content: space-evenly;
        list-style: none;
    }

    & ul li a{
        text-decoration: none;
        color: white;
        display: flex;
        align-items: center;
    }

    & ul li a img{
        height: 45px;
        margin-right: 20px;
    }
}
</style>