<template>
  <div class="wrap">
      <div class="content">
         <h1> Content Here </h1>

      </div>
  </div>
</template>

<script>
export default {
    name: "Content",
}
</script>

<style lang="scss" scoped>
@import '../style/variable.scss';
.wrap{
    height: 100px;
    background-color: $darker_black;
    .content{
        width: 90%;
        margin: 0px auto;
        padding: 10px 0;
        text-align: left;
        h1{
            font-size: 2.5rem;
            color: white;
        }
    }

}
</style>