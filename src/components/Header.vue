<template>
  <header>
      <!-- <div class="test">div</div> -->
    <div class="wrap">
        <div class="logo">
            <img src="../assets/images/dc-logo.png" alt="logo dc header">
        </div>
        <ul>
            <li v-for="(link,index) in links" :key=index :class="{'underline' : link.active}"> <a :href="link.url" @click="attiva(index)" :class="{'colored' : link.active}">{{link.text}}</a> </li>
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
                   text: "Characters",
                   url : "#",
                   active: false
               },
               {
                    text: "Comics",
                    url : "#",
                    active: true
               },
               {
                    text: "Movies",
                    url : "#",
                    active: false
               },
               {
                    text: "Tv",
                    url : "#",
                    active: false
               },
               {
                    text: "Games",
                    url : "#",
                    active: false
               },
               {
                    text: "Collectibles",
                    url : "#",
                    active: false
               },
               {
                    text: "Videos",
                    url : "#",
                    active: false
               },
               {
                    text: "Fans",
                    url : "#",
                    active: false
               },
               {
                    text: "News",
                    url : "#",
                    active: false
               },
               {
                    text: "Shop",
                    url : "#",
                    active: false
               },
           ] 
        }
    },
    methods:{
        attiva(index){
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
@import '../style/variable.scss';
    header{
        min-height: 70px;
        font-weight: bold;
        font-size: 18px;
        background-color: white;
        margin-top: 40px;
        .wrap{
            width: 90%;
            margin: 0 auto;
            display: flex;
            align-items: center;
            justify-content: space-between;
            .logo{
                margin: 20px 0px;
                img{
                    height: 80px
                };
            }
            ul{
                padding-top: 52px;
                text-transform: uppercase;

                li{
                    display: inline-block;
                    margin: 0px 20px;
                    padding-bottom: 52px;
                    position: relative;
                   
                }
            
            }
            
        }
    }
    .underline::after{
       display: block;
       content: '';
       height: 5px;
       background-color: $my_blue;
       width: 100%;
       position: absolute;
       bottom: 0;
    }
    .colored{
        color: $my_blue;
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
