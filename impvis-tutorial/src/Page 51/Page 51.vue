<template>
    <div>
        <iv-title-bar>ImpVis Tutorial</iv-title-bar>
        <iv-visualisation>
            <center>
            <h1>ImpVis Components Documentation Library</h1>
            </center>

            <div style="margin-left:10vw; background-color:grey; width:20vw;">
                <center><h2><u>Contents</u></h2></center>
                <h4>
                    <a href="#layoutComponents">Layout Components</a>
                </h4>
                <ul>
                    <a href="#pane">Pane</a>
                </ul>
                <ul>
                    <a href="#fixedHotspot">FixedHotspot</a>
                </ul>
                <ul>
                    <a href="#toggleHotspot">ToggleHotspot</a>
                </ul>
                <ul>
                    <a href="#titleBar">TitleBar</a>
                </ul>
                <ul>
                    <a href="#guidance">Guidance</a>
                </ul>
                <ul>
                    <a href="#sidebarSection">Sidebar Section</a>
                </ul>
                <ul>
                    <a href="#sidebarContent">Sidebar Content</a>
                </ul>                
            </div>
            
            <div style="margin-left: 5vw;">
                <h2 id="layoutComponents">Layout Components</h2>
                <h4 id="pane">Pane</h4>
                <h4 id="pane">Pane</h4>
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
    name:"Page51",
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

.red 
{ 
    color: red; 
} 


</style>



