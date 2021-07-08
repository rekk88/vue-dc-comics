<template>
  <div class="gallery_wrap">
     <!-- <span>{{comic.thumb}} gallery</span> -->
     <img :src="comic.thumb" :alt="fumetto">
     <span>{{comic.series}}</span>
  </div>
</template>

<script>
export default {
    name:"Gallery",
    props:["comic"]
}
</script>

<style lang="scss" scoped>
    .gallery_wrap{
        // height: 80px;
        width: calc(100% / 6);
        padding: 20px;
        img{
            width: 100%;
        }
    }
</style>