<script>
export default {
  name: "AppCard",
  data() {
    return {};
  },
  props: {
    img: String,
    title: String,
  },
}
</script>

<template>
  <div class="card">
    <div class="img-card-container">
      <img :src="img" alt="">
    </div>
    <div class="card-title">
      {{ title }}
    </div>
  </div>
</template>

<style lang="scss">

.card {
  display: flex;
  flex-direction: column;
  width: 200px;
  height: 250px;
  .img-card-container{
    width: 100%;
    height: 100%;
    background-color: blue;
    overflow: hidden;
    img {
      width: 100%;
      
    }
  }

  .card-title {
    text-transform: uppercase;
    padding-top: 10px;
  }
}

</style>