<template>
  <header>
      <!-- <div class="test">div</div> -->
    <div class="wrap">
        <div class="logo">
            <img src="../assets/images/dc-logo.png" alt="logo dc header">
        </div>
        <ul>
            <!-- <li>Item1</li>
            <li>Item2</li>
            <li>Item3</li> -->
            <li v-for="(link,index) in links" :key=index :class="{'underline' : link.active}"> <a :href="link.url" @click="attiva(link,index)" :class="{'colored' : link.active}">{{link.text}}</a> </li>
        </ul>
    </div>
  </header>
</template>

<script>
export default {
    name:"Header",
    data() {
        return {
           links:[
               {
                   text: "Item1",
                   url : "#",
                   active: false
               },
               {
                    text: "Item1",
                    url : "#",
                    active: false
               },
               {
                    text: "Item1",
                    url : "#",
                    active: false
               }
           ] 
        }
    },
    methods:{
        attiva(link,index){
            console.log(this.links);
            this.links.forEach((element,i) =>{
                if(index == i){
                    element.active = !element.active
                }
                else{
                    element.active = false
                }
            })
        }
    }
}
</script>

<style lang="scss" scoped>
    header{
        min-height: 70px;

        .wrap{
            background-color: lightblue;
            display: flex;
            align-items: center;
            justify-content: space-around;
            .logo{
                margin: 20px 0px;
                img{
                    height: 70px
                };
            }
            ul{
                padding-top: 20px;

                li{
                    display: inline-block;
                    margin: 0px 10px;
                    padding-bottom: 20px;
                    position: relative;
                   
                }
            
            }
            
        }
    }
    .underline::after{
       display: block;
       content: '';
       height: 5px;
       background-color: blue;
       width: 100%;
       position: absolute;
       bottom: 0;
    }
    .colored{
        color: blue;
    }
    // li:after{
    //     content: '';
    //     height: 5px;
    //     color: blue;
    //     width: 10px;
    //     position: absolute;
    //     bottom: 0;
    // }
</style>
