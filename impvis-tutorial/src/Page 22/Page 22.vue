<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <div class="iv-main">
                <center>
                <h1>2b1. Live server</h1>
                </center>
                <p>It is often convenient to see changes on your website while editing. For that purpose, we make use of the live server.
                Click on the extension button, search for Live Server, and install it.</p>
                <img src="@/assets/images/live_server.png"  style="width:80%;height:auto;"/>
                <p>Once you have done that, go back to the HTML file you have created and click on the <i>‘Go Live’</i> button on the bottom right.</p>
                <img src="@/assets/images/Hello_world.png"  style="width:80%;height:auto;"/>
                <p>Your HTML file will be opened in your default browser now. You can put the browser and VSCode side by side and see the changes 
                being done live (after saving your changes). You may utilise the autosave function (in the File dropdown) if you like.<br></p>
                <img src="@/assets/images/Hello_world_display.png"  style="width:80%;height:auto;"/>
                <p>To stop the Live Server, click on the ‘Port: 5500’ cancel button (at the bottom right).</p>
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
    name:"Page22",
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



