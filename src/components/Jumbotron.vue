<template>
  <div class="jumbo_wrap">
      <div class="series_button">Current Series</div>
  </div>
</template>

<script>
export default {
    name:"Jumbotron"
}
</script>
 
<style lang="scss" scoped>
.jumbo_wrap{
    background-image: url(../assets/images/jumbotron.jpg);
    background-position: top right;
    background-size: cover;
    height: 500px;
    position: relative;
    .series_button{
        background-color: blue;
        color: white;
        padding: 5px;
        position: absolute;
        bottom: 0;
        left: 10%;
        transform: translate(+100% , +50%);

    }
}
</style>