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

<template>
    <div class="bg-gray-100 bg-[url(https://wallpaperaccess.com/full/1558517.jpg)] ">
        <div class="container mx-auto">
            <Header :links="links" :changePage="changePage" :activePage="activePage"/>
            <div class="min-h-[50vh]  flex flex-col gap-4 items-start justify-center text-white">
                <h1 class="text-7xl drop-shadow-md font-bold">مكتب
                    ذ. رشيد لبرود</h1>
                <h4>مفوض قضائي لدى الدائرة القضائية بمراكش</h4>
                <button class="btn bg-red-500 border-none text-white hover:bg-red-600">احجز موعد الآن</button>
            </div>
        </div>
    </div>
</template>
