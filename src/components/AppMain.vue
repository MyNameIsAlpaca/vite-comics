<script>
export default {
  data() {
    return{
        content: "--> Content goes here <---",
    }
  },
  methods: {
  }
}

</script>

<template>
  <div class="main-container">
    <div class="container">
        <h2> {{ content }} </h2>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.main-container {
    background-color: #1c1c1c;
    color: white;
    .container {
        max-width: 1200px;
        margin: auto;
        h2 {
            padding: 50px;
        }
    }
}
</style>