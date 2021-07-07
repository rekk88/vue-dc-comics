<template>
  <div class="wrap">
      <!-- <div>{{pippo.src}} -  {{pippo.descrizione}}</div> -->
      <img :src="pippo.src" :alt="pippo.descrizione">
      <span>{{pippo.descrizione}}</span>
  </div>
</template>

<script>
export default {
    name:"LinksCard",
    props:["pippo"]
}
</script>

<style lang="scss" scoped>
    .wrap{
        margin: 0px 30px;
        img{
            vertical-align: middle;
            height: 70px;
            padding: 5px;
        }
        span{
            text-transform: uppercase;
            color: white;
            margin-left: 5px;
        }
    }
    
</style>