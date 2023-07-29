<template>
    <Banner :changePage="changePage" :links="links" :activePage="activePage"/>
    <AboutUsSection/>
    <Certificates/>
    <Ser/>
    <HowTo/>
</template>
<script>
    import Banner from "../components/Banner.vue"
    import AboutUsSection from "../components/AboutUsSection.vue"
    import Certificates from "../components/Certificates.vue"
    import Ser from "../components/Ser.vue"
    import HowTo from "../components/HowTo.vue"
    export default {
        props:["links","activePage","changePage"],
        components:{
                Banner,
                AboutUsSection,
                Certificates,
                Certificates,
                Ser,
                HowTo
            }
    }
</script>