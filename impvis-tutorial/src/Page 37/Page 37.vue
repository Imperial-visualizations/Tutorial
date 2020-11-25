<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <div class="iv-main">
            <center>
            <h1>4b. The ImpVis Visual Identity -  Text</h1>
            </center>
            Imperial College London’s executive typeface “Meta normal” is used as the font on all visualisations. For more information on this, see:
            <a href="https://www.imperial.ac.uk/brand-style-guide/visual-identity/font/">https://www.imperial.ac.uk/brand-style-guide/visual-identity/font/</a>
            You can refer to “Notes_on_format_for_clarity_and_comprehension.pdf” in this repository for more details.
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
    name:"Page37",
}
</script>
<style>
.iv-main{
    margin:10px 50px;
}
 ul {
  list-style-type: none;
 }

 code {
    background-color: #eee;
    border-radius: 3px;
    font-family: courier, monospace;
    padding: 0 3px;
}



</style>



