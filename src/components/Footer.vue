<template>
  <div class="footer_wrap">
      <div class="top">
          <div class="content">
            <div class="left">
                <div class="list1">
                    <ul>
                        <li><h2>DC Comics</h2></li>
                        <li>Lista 1</li>
                        <li>Lista 1</li>
                        <li>Lista 1</li>
                    </ul>
                    <ul>
                        <li><h2>shop</h2></li>
                        <li>Lista 4</li>
                        <li>Lista 4</li>
                        <li>Lista 4</li>
                        <li>Lista 4</li>
                        
                    </ul>
                </div>
                <div class="list2">
                    <ul>
                    <li><h2>DC</h2></li>
                    <li>Lista 2</li>
                    <li>Lista 2</li>
                    <li>Lista 2</li>
                    <li>Lista 2</li>
                    <li>Lista 2</li>
                    <li>Lista 2</li>
                    <li>Lista 2</li>
                    <li>Lista 2</li>
                    <li>Lista 2</li>
                    </ul>

                </div>
                <div class="list3">
                    <ul>
                    <li><h2>Sites</h2></li>
                    <li>Lista 3</li>
                    <li>Lista 3</li>
                    <li>Lista 3</li>
                    <li>Lista 3</li>
                    
                    </ul>
                </div>
            </div>
            <div class="righ">
            </div>
          </div>
        
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
        // display: flex;
        // flex-wrap: wrap;
        // flex-grow: 1;
        text-align: left;
        .top{
            // height: 390px; /*altezza da togliere*/
            width: 100%;
            background-image: url("../assets/images/footer-bg.jpg");
            background-position: center top;
            background-repeat: no-repeat;
            background-size: cover;
            .content{
                width: 90%;
                margin: 0 auto;
                background-image: url("../assets/images/dc-logo-bg.png");
                background-repeat: no-repeat;
                background-position: right;
                .left{
                    display: flex;
                    padding: 80px 0px;
                    .list1 ul:nth-child(2){
                        padding-top: 10px;
                    }
                    .list2{
                        margin: 0px 60px;
                    }
                }
                .left ul li{
                    list-style: none;
                }
                 .left ul li h2{
                     color: white;
                }
                .right{

                }
            }
        }
        .bottom{
            // height: 100px;
            width: 100%;
            //127+41+100+150+390 somma altezze
            height: calc(100vh - 788px); //un pò spartana come soluzione ma ho esaurito le opzioni
            background-color: lightblue;
        }
    }
</style>