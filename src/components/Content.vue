<template>
  <div class="wrap">
      <div class="content">
        <!-- <h1> Content Here </h1> -->
        <Jumbotron /> 
        <div class="gallery_container">
            <Gallery v-for="(item,index) in cazzabubboli" :key="index" :comic="item"/>
        </div>
      </div>
  </div>
</template>

<script>
import Jumbotron from './Jumbotron.vue'
import Gallery from './Gallery.vue'
import Comics from '../data/Comics.js'

export default {
    name: "Content",
    components:{
        Jumbotron,
        Gallery
    },
    data() {
        return {
            cazzabubboli:Comics
        }
    },
    mounted() {
    //   console.log(fumetti);
    },
}
</script>

<style lang="scss" scoped>
@import '../style/variable.scss';
.wrap{
    min-height: 500px;
    background-color: $darker_black;
    .content{
        // width: 90%;
        // margin: 0px auto;
        // padding: 10px 0;
        text-align: left;
        // height: 100%;
        h1{
            font-size: 2.5rem;
            color: white;
        }
        .gallery_container{
            display: flex;
            flex-wrap: wrap;
            width: 80%;
            margin: 0 auto;
            justify-content: space-around;
        }
    }

}
</style>