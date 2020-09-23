<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <template #hotspots>
                <iv-pane position="left">
                    Hi! This is a pane
                </iv-pane>
            </template>
            <center>
            <h1> Panes</h1>
            </center>
            Here is a screenshot of some code used to make a pane using the ImpVis library.
             <img src="@/assets/images/pane_code.png"  style="width:518px;height:298px;" align = "right"/>
             This code produces what you see onscreen now, a pane attached to the left of the screen with the text "Hi! This is a pane"
             on the inside.
        </iv-visualisation>
    </div>
</template>
<script>
import {name} from '../package.json';

export default {
    name:"Page",
    
    data(){
        return {
            projectName: name
        }
    },
}
</script>
<style>
div {
  padding-top: 10px;
  padding-bottom: 50px;
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



