<script>
export default {
  data() {
    return{
        links: [
            {
                title: "characters",
            },
            {
                title: "comics",
            },
            {
                title: "movies",
            },
            {
                title: "tv",
            },
            {
                title: "games",
            },
            {
                title: "collectibles",
            },
            {
                title: "videos",
            },
            {
                title: "fans",
            },
            {
                title: "news",
            },
            {
                title: "shop",
            },
        ],
        activeIndex: 0,
    }
  },
  methods: {
    changeActiveIndex(index) {
        this.activeIndex = index;
    }
  }
}

</script>

<template>
  <div class="main-container">
    <div class="logo-img">
        <img src="/img/dc-logo.png" alt="logo dc">
    </div>
    <div class="navLinks">
        <ul>
            <li :class="index == activeIndex ? 'active' : ''" @click="changeActiveIndex(index)" v-for="(link, index) in links">{{ link.title }}</li>
        </ul>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.main-container {
    max-width: 1200px;
    margin: auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 0;
    .logo-img {

        img{
            max-width: 90%;
        }
    }
    .navLinks ul {
        display: flex;
        li{
            padding: 10px;
            font-weight: 600;
            text-transform: uppercase;
            cursor: pointer;
            &.active {
                color: #0c7cec;
                position: relative;
            }

            &.active::before {
                display: block;
                content: "";
                width: 70%;
                height: 10px;
                background-color: #0c7cec;
                position: absolute;
                bottom: -48px;
            }
        }
    }
}



</style>
