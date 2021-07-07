<template>
  <div class="wrap">
      <!-- <div>{{pippo.src}} -  {{pippo.descrizione}}</div> -->
      <img :src="pippo.src" :alt="pippo.descrizione">
  </div>
</template>

<script>
export default {
    name:"LinksCard",
    props:["pippo"]
}
</script>

<style lang="scss" scoped>

</style>