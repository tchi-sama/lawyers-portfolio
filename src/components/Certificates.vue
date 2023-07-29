<template>
    <div class="container mx-auto py-8 my-8">
        <h1 class="text-4xl font-bold">الديبلومات و الشواهد</h1>
        <div class="flex gap-4 py-10">
            <div class="rounded-xl bg-white flex flex-col gap-2 shadow-xl p-8 flex-1" v-for="certificate in certificates" :key="certificate.year">
                <h4 class="text-xl font-bold">{{ certificate.year }}</h4>
                <h2 class="text-2xl font-bold">{{ certificate.type }}</h2>
                <p>{{ certificate.description }}</p>
            </div>
        </div>
    </div>
</template>
<script>
    export default{
        name:"certificates",
        data(){
            return{
                certificates:[
                    {year:2000,type:'الديبلوم',description:"خريج المعهد العالي للقضاء بالرباط."},
                    {year:2008,type:'الشهادة',description:"شهادة الاهلية لمزاولة مهنة المحاماة."},
                    {year:2015,type:'الإجازة',description:"الإجازة في القانون الخاص بجامعة القاضي عياض بمراكش."},
                ]
            }
        }
    }
</script>