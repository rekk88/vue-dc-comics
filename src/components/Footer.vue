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
            <span class="sign_up">sign-up now!</span>
            <div>
                <span>
                    follow us
                    <img src="../assets/images/footer-facebook.png" alt="">
                    <img src="../assets/images/footer-facebook.png" alt="">
                    <img src="../assets/images/footer-facebook.png" alt="">
                    <img src="../assets/images/footer-facebook.png" alt="">
                    <img src="../assets/images/footer-facebook.png" alt="">

                </span>
            </div>
      </div>
  </div>
</template>

<script>
export default {
    name:"Footer.vue",


}
</script>
 
<style lang="scss" scoped>
@import '../style/variable.scss';

    .footer_wrap{
        // display: flex;
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
              
            }
        }
        .bottom{
            // height: 100px;
            //127+41+100+150+390 somma altezze
            width: 90%;
            height: calc(100vh - 788px); //un pò spartana come soluzione ma ho esaurito le opzioni
            // background-color: lightblue;
            display: flex;
            align-items: center;
            justify-content: space-between;
            margin: 0 auto;

            span.sign_up{
                display: inline-block;
                border: 3px solid $my_blue;
                padding: 7px;
                font-size: 17px;
                text-transform: uppercase;
            }
            div{
                display: inline-block;
                span{
                    font-size: 19px;
                    text-transform: uppercase;
                    color: $my_blue;
                    font-weight: bold;
                    img{
                        vertical-align: middle;
                        margin:0px 5px;
                    };
                }
            }
        }
    }
</style>