<script>
export default {
  data() {
    return{
        leftLinksColumn: [
            {
                title: "dc comics",
                linkUrl: [
                   "Characters",
                   "Comics",
                   "Movies",
                   "Tv",
                   "Games",
                   "Videos",
                   "News" 
                ]
            },
            {
                title: "shop",
                linkUrl: [
                   "Shop DC",
                   "Shop DC Collectibles",
                ]
            }
        ],

        rightLinksColumn: [
            {
                title: "dc",
                linkUrl: [
                   "Terms Of Use",
                   "Privacy policy (New)",
                   "Ad Choices",
                   "Advertising",
                   "Jobs",
                   "Subscriptions",
                   "Talent Workshops", 
                   "CPSC Certificates",
                   "Ratings",
                   "Shop Help",
                   "Contact Us",
                ]
            },
            {
                title: "sites",
                linkUrl: [
                   "DC",
                   "MAD Magazine",
                   "DC Kids",
                   "DC Universe",
                   "DC Power Visa",
                ]
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
            <div class="column">
                <div class="leftColumn">
                    <div v-for="(link, index) in leftLinksColumn">
                        <strong>{{link.title}}</strong>
                        <ul> 
                            <li v-for="linkaUrl in leftLinksColumn[index].linkUrl">
                                {{ linkaUrl }}
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="rightColumn">
                    <div v-for="(link, index) in rightLinksColumn">
                        <strong>{{link.title}}</strong>
                        <ul> 
                            <li v-for="linkaUrl in rightLinksColumn[index].linkUrl">
                                {{ linkaUrl }}
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
                <img src="/img/dc-logo-bg.png" alt="">
        </div>
    </div>
</template>

<style lang="scss" scoped>
.main-container{
    width: 100%;
    background-image: url(/img/footer-bg.jpg);
    .container{
        max-width: 1200px;
        max-height: 400px;
        margin: auto;
        color: white;
        display: flex;
        justify-content: space-between;
        img {
            object-fit: cover;
        }
        .column{
            padding: 80px 0;
            display: flex;
            gap: 40px;
            .leftColumn {
                display: flex;
                flex-direction: column;
                gap: 10px;
                div {
                    display: flex;
                    flex-direction: column;
                    gap: 5px;
                    strong {
                        text-transform: uppercase;
                        font-size: 1.2em;
                    }
                    li {
                        color: gray;
                        font-size: 0.8em;
                    }
                }
            }
    
            .rightColumn {
                display: flex;
                gap: 40px;
                div {
                    display: flex;
                    flex-direction: column;
                    gap: 5px;
                    strong {
                        text-transform: uppercase;
                        font-size: 1.3em;
                    }
                    li {
                        color: gray;
                        font-size: 0.8em;
                    }
                }
            }
        }
    }
}
</style>