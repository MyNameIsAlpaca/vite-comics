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
  <div class="containerCard">
    <div class="card">
      <div class="img-card-container">
        <img :src="img" alt="">
      </div>
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
    aspect-ratio: 1/1;
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