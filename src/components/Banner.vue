<template>
    <div class="bg-red-400">
        <Header :links="links" :changePage="changePage" :activePage="activePage"/>
        <div class="min-h-[50vh]">
            <h1 class="text-5xl">tchisama a programer</h1>
            <h4 class="text-xl">Lorem ipsum dolor sit amet consectetur adipisicing elit. Qui ullam placeat magni mollitia laborumramer</h4>
        </div>
    </div>
</template>
<script>
    import Header from "./Header.vue"
    export default{
        name:"banner",
        props:["links","activePage","changePage"],
        components:{
            Header
        }
    }
</script>