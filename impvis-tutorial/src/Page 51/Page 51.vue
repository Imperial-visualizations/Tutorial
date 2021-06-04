<template>
    <div>
        <iv-title-bar style="z-index:2;">ImpVis Tutorial</iv-title-bar>
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
                    <a href="#sidebarContent">Sidebar Content</a>
                </ul>  
                <ul>
                    <a href="#sidebarSection">Sidebar Section</a>
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
              
            </div>
            
            <div style="margin-left: 5vw;">
                <h2 id="layoutComponents">Layout Components</h2>
                <h4 id="pane">Pane</h4>
                Creates a container on the side of the page which can house content, usually text.
                <br>
                <img src="./assets/Pane.png">
                <h5>Props</h5>
                Name: width <br>
                Type: Number <br>
                Default: 200 <br>
                Description: The defualt width of the pane. (May be resized by user) <br><br>

                Name: format <br>
                Type: String <br>
                Default: 'push' <br>
                Description: Determines the behaviour of the pane. <br>
                Possible Values: 'push', 'full', 'overlay' <br><br>

                Name: opacity <br>
                Type: Number <br>
                Default: 0 <br>
                Description: Determines how transparent the pane is. <br><br>


                <h4 id="sidebarContent">Sidebar Content</h4>
                Place inside pane component. Wraps text.
                <br>
                <img src="./assets/SidebarContent.png">
                <h5>Props</h5>
                Name: showPagination <br>
                Type: Bool <br>
                Default: "true" <br>
                Description: <br><br>


                <h4 id="sidebarSection">Sidebar Section</h4>
                Place inside "sidebar Content" component. Creates a title with an icon for a section of text and adds the section to navigation.
                <br>
                <img src="./assets/SidebarSection.png">
                <h5>Props</h5>
                Name: highlight <br>
                Type: Bool <br>
                Default: "false" <br>
                Description: If true, highlights all text in the section with the theme colour. default=false. <br><br>

                Name: icon <br>
                Type: String <br>
                Default: "star" <br>
                Description: The icon displayed for the section. <br>
                Possible Values: <a href="https://fontawesome.com/v5.15/icons?m=free">these</a> <br><br>

                Name: theme <br>
                Type: String <br>
                Default: "blue" <br>
                Description: The colour theme for the section. <br><br>

                Name: title <br>
                Type: String <br>
                Description: The title of the section <br><br>


                <h4 id="fixedHotspot">Fixed Hotspot</h4>
                Container for HTML within a certain section of the screen.
                <br>
                <img src="./assets/FixedHotspot.png">
                <h5>Props</h5>
                Name: position <br>
                Type: String <br>
                Description: The position on the screen the fixed hotspot will be placed in. <br>
                Possible Values: "left", "right", "top", "bottom", "topleft", "topright", "bottomright", "bottomleft" <br><br>

                Name: size <br>
                Type: Number <br>
                Default: -1 <br>
                Description: Set the explict size on the major axis of the hotspot, if set to -1 (default) will fill all available space. <br><br>

                Name: noWastedSpace <br>
                Type: Bool <br>
                Default: "false" <br><br>

                Name: transparent <br>
                Type: Bool <br>
                Default: "false" <br><br>

                Name: glass <br>
                Type: Bool <br>
                Default: "false" <br><br>


                <h4 id="toggleHotspot">Toggle Hotspot</h4>
                Container for HTML within a certain section of the screen, which may be hidden or displayed with a tab.
                <br>
                <img src="./assets/ToggleHotspot1.png">
                <img src="./assets/ToggleHotspot2.png">
                <h5>Props</h5>
                Name: position <br>
                Type: String <br>
                Description: The position on the screen the fixed hotspot will be placed in. <br>
                Possible Values: "left", "right", "top", "bottom", "topleft", "topright", "bottomright", "bottomleft" <br><br>

                Name: title <br>
                Type: String <br>
                Description: The text which will be displayed on the tab. <br><br>

                Name: size <br>
                Type: Number <br>
                Default: -1 <br>
                Description: Set the explict size on the major axis of the hotspot, if set to -1 (default) will fill all available space. <br><br>

                Name: noWastedSpace <br>
                Type: Bool <br>
                Default: "false" <br><br>

                Name: glass <br>
                Type: Bool <br>
                Default: "false" <br><br>

                Name: show <br>
                Type: Bool <br>
                Default: "false" <br><br>



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



