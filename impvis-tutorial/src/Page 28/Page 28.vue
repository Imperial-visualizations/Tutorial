<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <template #hotspots>
                <iv-pane position="left">
                    Hi! This is a pane
                </iv-pane>
                <iv-toggle-hotspot position="bottom" title = "Button Title">
                    This will go in the pop-out section!
                </iv-toggle-hotspot>
            </template>
            <div class="iv-main">
            <center>
            <h1>Toggleable Hotspots</h1>
            </center>
            The impvis library also has <i>hotspots</i> which can either be toggleable or fixed. Here is some example code
            for producing a toggleable hotspot on the bottom of the page that had the Pane on it.
             <img src="@/assets/images/hotspot_text_code.png"  style="width:518px;height:298px;" align = "right"/>
             Notice how the hotspot overlays over the main content of the visualisation. We will later discuss how
             to use this feature effectively when designing the learning journey for the users of your visualisations.
            </div>

        </iv-visualisation>
    </div>
</template>
<script>
export default {
    name:"Page28",
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



