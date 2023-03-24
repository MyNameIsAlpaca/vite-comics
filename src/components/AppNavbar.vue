<script>
export default {
  data() {
    return{
        links: [
            {
                title: "digital comics",
                picture: "/img/buy-comics-digital-comics.png"
            },
            {
                title: "dc merchandise",
                picture: "/img/buy-comics-merchandise.png"
            },
            {
                title: "subscription",
                picture: "/img/buy-comics-subscriptions.png"
            },
            {
                title: "comic shop locator",
                picture: "/img/buy-comics-shop-locator.png"
            },
            {
                title: "dc power visa",
                picture: "/img/buy-dc-power-visa.svg"
            },
        ]
    }
  },
  methods: {
  }
}

</script>

<template>
  <div class="main-container">
    <div class="container">
        <ul>
            <li v-for="link in  links">
                <div class="img-container">
                    <img :src="link.picture" alt="">
                </div>
                {{ link.title }}
            </li>
        </ul>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.main-container {
    background-color: #0282f9;
    color: white;
    .container {
        max-width: 1200px;
        margin: auto;
        ul{
            display: flex;
            justify-content: space-around;
            li{
                text-transform: uppercase;
                display: flex;
                padding: 40px 0;
                align-items: center;
                gap: 10px;
                .img-container {
                    max-width: 50px;
                    max-height: 50px;
                    img{
                        width:  100%;
                        max-height: 50px;
                    }
                }
            }
        }
    }
}
</style>