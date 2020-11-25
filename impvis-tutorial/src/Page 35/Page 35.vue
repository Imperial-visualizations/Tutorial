<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <div class="iv-main">
            <center>
            <h1>4b. The ImpVis Visual Identity - Colour Schemes</h1>
            </center>
            <p>When developing the colour scheme for any individual visualisation, special attention should be 
                paid to keeping the visualisations colour-blind friendly. In practice, this means making fair 
                use of monochromatic schemes when possible and using online tools to ensure that, when contrasting 
                colours are chosen (e.g., in plots), they are visibly contrasting to everyone. Some useful links are:
                <a href="http://colorbrewer2.org/#type=sequential&scheme=BuGn&n=3">http://colorbrewer2.org/#type=sequential&scheme=BuGn&n=3</a> and 
                <a href = "https://venngage.com/blog/color-blind-friendly-palette/">https://venngage.com/blog/color-blind-friendly-palette/</a>
            </p>

            <p>
                Currently, we have two primary colours for the lay-out components, the Imperial Blue (#133f6f) and the 
                Hotspot Orange (#FF901C). These are used in the Title bar and hotspot button components, respectively. 
                Within components such as the sliderBlock, we advise using different shades and tints of a single colour 
                to create a distinction between subsections within a component and combining with the help of black and 
                white text depending on the given background colour. The sliderBlock shown below highlights this.
            </p><img src="@/assets/images/sliderblock.png"  style="width:374px;height:auto;" align = "center"/>
            
            <p> We want the developer to have freedom in picking colours for their components but within a range of colour choices 
                that are not too wide in breadth. This specific range is currently set by the following:
            </p><img src="@/assets/images/colour_scheme.png"  style="width:1380px;height:auto;" align = "center"/>
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
    name:"Page35",
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