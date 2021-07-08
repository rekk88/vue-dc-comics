<template>
  <div class="footer_wrap">
      <div class="top">

      </div>
      <div class="bottom">
           un div 
      </div>
  </div>
</template>

<script>
export default {
    name:"Footer.vue",


}
</script>
 
<style lang="scss" scoped>
    .footer_wrap{
        display: flex;
        flex-wrap: wrap;
        flex-grow: 1;
        .top{
            height: 390px; /*altezza da togliere*/
            width: 100%;
            background-image: url("../assets/images/footer-bg.jpg");
            background-position: center top;
            background-repeat: no-repeat;
            background-size: cover;
        }
        .bottom{
            // height: 100px;
            width: 100%;
            height: calc(100vh - 807px); //un pò spartana come soluzione ma ho esaurito le opzioni
            background-color: lightblue;
        }
    }
</style>