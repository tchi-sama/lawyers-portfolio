<script>
    export default{
        name:"header",
        props:["links","activePage","changePage"],
        methods:{
            changePageTo(i){
                this.changePage(i)
            }
        }
        
    }
</script>

<template>
    <div class="py-4 flex">
        <div class="container mx-auto flex flex-row-reverse items-center justify-between">
            <div>
                <img src="" alt="">
                <h3 class="text-xl font-bold text-white uppercase">Logo name</h3>
            </div>
            <div class="flex gap-2 ">
                <button 
                    v-for="(link,i) in links" 
                    :key="i" 
                    @click="changePageTo(i)" 
                    :class="i==activePage?'text-white font-bold':'text-gray-200'"
                    class="font-medium border-none bg-transparent p-2 btn hover:bg-[#fff2]"
                    >{{ link.name }}</button>
            </div>
        </div>
    </div>
</template>