<template>
    <div>
        <MenuStyle1 />
        <PageHeader pageTitle="Call For Papers" parentPage="For Authors" />
        <CallForPaperComponentVue/>
        <Footer />
    </div>
  
</template>

<script>
import MenuStyle1 from '@/components/layout/MenuStyle1'
import PageHeader from '@/components/layout/PageHeader'
import CallForPaperComponentVue from '../components/page_components/for_authors/CallForPaperComponent.vue'
import Footer from '@/components/layout/Footer'
export default {
    name : "Blogs",
    components : {
        MenuStyle1,
        PageHeader,
        CallForPaperComponentVue,
        Footer
    }

}
</script>

<style>

</style>