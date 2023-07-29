<template>
    <Banner :changePage="changePage" :links="links" :activePage="activePage"/>
</template>
<script>
    import Banner from "../components/Banner.vue"
    export default {
        props:["links","activePage","changePage"],
        components:{
            Banner,
        }
    }
</script>