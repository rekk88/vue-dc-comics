<template>
  <header>
      <!-- <div class="test">div</div> -->
    <div class="wrap">
        <div class="logo"></div>
        <ul>
            <li>Item1</li>
            <li>Item2</li>
            <li>Item3</li>
        </ul>
    </div>
  </header>
</template>

<script>
export default {
    name:"Header"
}
</script>

<style lang="scss" scoped>
    header{
        height: 70px;

        .wrap{
            background-color: lightblue;
            height: 100%;
            display: flex;
            align-items: center;
            justify-content: space-around;
            .logo{
                width: 50px;
                height: 100%;
                background-color: lightseagreen;
            }
            li{
                display: inline-block;
            }
        }
    }
</style>
