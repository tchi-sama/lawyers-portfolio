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
    <div class="">
        <div class="flex gap-2">
                <button v-for="(link,i) in links" :key="i" class="p-2" @click="changePageTo(i)" :class="i==activePage?'bg-white':'bg-transparent'" >{{ link.name }}</button>
        </div>
    </div>
</template>