<template>
  <div dir="rtl" class="bg-gray-100">
    <Home :changePage="changePage" :links="links" :activePage="activePage"/>
  </div>
</template>

<script>
import Home from "./pages/home.vue"
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
      Home
    }
}
</script>


