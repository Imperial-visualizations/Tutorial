<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <div class="iv-main">
  <center>
            <h1>Importing your own components</h1>
            </center>
            <p>Say you wanted to create your own component that does its own thing, you can import this as a separate file and
                use it in your visualisations. 
             <img src="@/assets/images/mainstage_location.png"  style="width:422px;height:auto;" align = "left"/>
             In order to use the file (which we will call MainStage.vue for now), you must export it. Everything you might 
             want to use outside of the MainStage.vue file is written in the export default code block.
             <img src="@/assets/images/mainstage_code.png"  style="width:256px;height:auto;" align = "right"/>
            </p>
            <p>
                For example, we might want to create a canvas that we can display some interactive content in (check out the SHM visualisation, we'll
                go through some of that content here). To do this, we'd write the following pieces of code: </p><br>
                <p> 1.) Place the input from mainstage into the correct part of template (where you want it to go) in App.vue (see image to the right)
                 <img src="@/assets/images/placing_mainstage.png"  style="width:438px;height:auto;" align = "right"/></p><br>
                 <p> 2.) Insert the code that draws a box around the edges of the canvas drawing area on the screen (that's what we currently
                     want to do, so we can see the canvas). (See image to the left).
                 <img src="@/assets/images/canvas_box.png"  style="width:408px;height:auto;" align = "left"/></p>
        <p> A screenshot of the result of this code is pasted below.
               <img src="@/assets/images/canvas_box_display.png"  style="width:690px;height:auto;" align = "center"/></p>
            </div>
          
        </iv-visualisation>
    </div>
</template>
<script>
export default {
    name:"Page32",
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



