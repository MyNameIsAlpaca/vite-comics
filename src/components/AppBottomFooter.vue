<script>
export default {
  data() {
    return{
        socialLinks: [
            {
                url: "",
                logo: "/img/footer-facebook.png"
            },
            {
                url: "",
                logo: "/img/footer-twitter.png"
            },
            {
                url: "",
                logo: "/img/footer-youtube.png"
            },
            {
                url: "",
                logo: "/img/footer-pinterest.png"
            },
            {
                url: "",
                logo: "/img/footer-periscope.png"
            }
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
            <button>SIGN-UP NOW!</button>
            <div class="socialContainer">
                <h2>FOLLOW US</h2>
                <ul>
                    <li v-for="(socialLogo, index) in socialLinks">
                        <img :src="socialLinks[index].logo" alt="">
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.main-container{
    background-color: #303030;
    .container{
        padding: 45.5px 0;
        max-width: 1200px;
        margin: auto;
        display: flex;
        align-items: center;
        justify-content: space-between;
        button {
            padding: 10px 20px;
            font-size: 15px;
            background-color: #303030;
            border: 1px solid #0282f9;
            color: white;
        }
        .socialContainer {
            display: flex;
            gap: 30px;
            align-items: center;
            h2 {
                color: #0282f9;
            }
            ul {
                display: flex;
                gap: 20px;
            }
        }
    }
}
</style>