<template>
    <Header/>
    <Footer/>
</template>

<script>
import Header from "@/components/Header";
import Footer from "@/components/Footer";
export default {
    name: "App",
    components: {Footer, Header}
}
</script>

<style lang="sass">
*
    box-sizing: border-box
    margin: 0

</style>