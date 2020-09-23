<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <center>
            <h1>2b1. Live server</h1>
            </center>
            <p>It is often convenient to see changes on your website while editing. For that purpose, we make use of the live server.
            Click on the extension button, search for Live Server, and install it.</p>
            <img src="@/assets/images/live_server.png"  style="width:277x;height:78x;"/>
            Once you have done that, go back to the HTML file you have created and click on the <i>‘Go Live’</i> button on the bottom right.
            <img src="@/assets/images/Hello_world.png"  style="width:1380x;height:783x;"/>
            Your HTML file will be opened in your default browser now. You can put the browser and VSCode side by side and see the changes 
            being done live (after saving your changes). You may utilise the autosave function (in the File dropdown) if you like.<br><center>
            <img src="@/assets/images/Hello_world_display.png"  style="width:1024x;height:132x;"/></center>
            To stop the Live Server, click on the ‘Port: 5500’ cancel button (at the bottom right).
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



