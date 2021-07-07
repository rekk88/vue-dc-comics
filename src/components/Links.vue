<template>
  <div class="wrap">
      <div class="content">
          <LinksCard v-for="(item,index) in shopLinks" :key="index" :pippo="item"/>
      </div>
  </div>
</template>

<script>
import Cards from '../data/Cards.js'
import LinksCard from './LinksCard.vue'
export default {
    name:"Links",
    components:{
        LinksCard
    },
    data() {
        return {
            shopLinks: Cards      
        }
    },
}
</script>

<style lang="scss" scoped>
@import '../style/variable.scss';
.wrap{
    background-color: $my_blue;
    .content{
        width: 90%;
        margin: 0px auto;
        /*debug */
        height: 200px;
        display: flex;
        align-items: center;
        justify-content: center;
    }
}

</style>