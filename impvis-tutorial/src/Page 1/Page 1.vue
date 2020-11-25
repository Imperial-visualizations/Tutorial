<template>
    <div>
        <iv-title-bar>ImpVis tutorial - Welcome</iv-title-bar>
        <iv-visualisation>
            <div class="intro-banner">
            <img src="@/assets/images/ImpVis-logo.png"/>
            
            <h1> Welcome to the ImpVis tutorial</h1>
            This is a document that aims to tell you everything you need to know, from start to finish, when creating a visualisation.<br> Check out the ImpVis website by clicking on the logo
            on the top right of the page.<br> 
            Please note, if you have any further questions, feel free to get in touch with Caroline Clewley at <a href="mailto:c.clewley@imperial.ac.uk">c.clewley@imperial.ac.uk</a>
            </div>
            <NavigationButton :pageName="this.$options.name" />
        </iv-visualisation>
    </div>
</template>
<script>
import NavigationButton from "../components/NavigationButton.vue";

export default {
    components: {
        NavigationButton,
    },
    name:"Page1",
}
</script>
<style>
.intro-banner{
    margin-top:20px;
    text-align: center;
}
</style>



