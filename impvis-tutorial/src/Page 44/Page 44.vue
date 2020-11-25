<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <div class="iv-main">
<center>
            <h1>Debugging and Console</h1>
            </center>
            <p>In Python, debugging is easy - you press play, and if there is an error in the code, your interpreter tells you precisely what and where it is. For web development, debugging is a little trickier, but the golden rule is F12 (or fn+F12 for some keyboards) is your best friend! This hotkey (or right-click + inspect for mac) brings up the browser developer tools, composed of several tabs. Of these, the elements tab is essentially your HTML/CSS debugger. If you hover over the HTML brought up in this tab, the div will be highlighted on the actual web page. Here we can see the div and its corresponding padding highlighted on the page when the container div is hovered over</p>
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
    name:"Page44",
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



