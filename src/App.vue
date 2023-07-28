<template>
  <Banner :changePage="changePage" :links="links" :activePage="activePage"/>
</template>

<script >
import Banner from './components/Banner.vue'
export default{
        data(){
            return{
                activePage:0,
                links:[
                    {name:"home",url:"/"},
                    {name:"about",url:"/about"},
                    {name:"contact",url:"/contact"},
                ]
            }
        },
        methods:{
            changePage(page){
                this.activePage=page;
            }
        },
        components:{
          Banner
        }
}
</script>


