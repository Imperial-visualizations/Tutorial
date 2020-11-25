<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <div class="iv-main">
<center>
            <h1>4b. The ImpVis Visual Identity - Colour Schemes (part 2)</h1>
            </center>
            <p>The range of shade and tints show below is achieved using two equations:
                <ul>
                    <li>New_rgb = old_r *(1 - shade_Factor), old_g *(1 - shade_Factor), old_b *(1 - shade_Factor)</li>
                    <li> New_rgb = old_r + (255 - old_r )*tint_Factor, old_g + (255 - old_g )*tint_Factor, old_b + (255 - old_b)*tint_Factor</li>
            </ul>
            The first equation produced darker shades, and the second equation made lighter tints, with the shade
            and tint factors in each varied to increase change. These colours and their shades are produced once at 
            the page load in <b>colorStore.js</b> vue bus and may be accessed by using <code>import colorStore from 
            "@/buses/colorStore"</code> the shades of a given colour are then selected using color: <code>colorStore.color_full_list["myColour"]</code>.  
            Note that the selectable colours are accessed using the following keys:
            <ul>
                <li>"navy": [14,64,111],</li>
                <li>"blue": [0,139,210],</li>
                <li>"teal": [17,177,162],</li>
                <li>"green": [168,204,106],</li>
                <li>"purple": [98,41,107],</li>
                <li>"berry": [207,16,63],</li>
                <li>"orange": [239,120,20],</li>
                <li>"tangerine": [246,176,15],</li>
                <li>"yellow": [252,217,22]</li>
            </ul>
            </p>
            <p>
                Where the RGB has replaced the hex codes for each colour for the colour. So for example, if I 
                wanted to access the shades for #0E406F (the first colour), then I would use: <code>color: colorStore.color_full_list[“navy”]</code> 
                within the data of my component and then to access a specific shade I use <code>this.color.shade_500</code> 
                (for the unchanged input navy colour), <code>this.color.shade_900</code>(for the darkest shade), 
                <code>this.color.shade_100</code>(for the lightest shade). For an example of components using the 
                colours see sliderBlock and guidanceModal.
            </p>
            <img src="@/assets/images/sliderblock_colours.png"  style="width:512px;height:auto;"/>
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
    name:"Page36",
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



