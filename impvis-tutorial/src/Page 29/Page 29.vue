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
                <iv-fixed-hotspot position="bottomright" title = "Fixed">
                    This will go inside the fixed hotspot, so will always appear on the screen.
                    P.S. You must specify a title and positione.
                </iv-fixed-hotspot>
            </template>
            <div class="iv-main">
                <center>
            <h1>Fixed-Hotspots</h1>
            </center>
            <p>Hotspots can also be fixed in position so that they <i>always</i> appear onscreen, as opposed to being toggleable
            where they can be brought on and off. For example now, to add a fixed hotspot to the code on the previous page,
            we could do
             <img src="@/assets/images/fixed_hotspot_code.png"  style="width:518px;height:auto;" align = "left"/>
             Notice how the hotspot overlays over the main content of the visualisation. We will later discuss how
             to use this feature effectively when designing the learning journey for the users of your visualisations.
            The screenshotted code would produce a fixed hotspot in the top right of the page. For this demonstration, I have displayed
                the hostspot in the bottom right for clarity.
            </p>
            </div>
          
        </iv-visualisation>
    </div>
</template>
<script>
export default {
    name:"Page29",
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



