<template>
    <div>
        <iv-title-bar style="z-index:2;">ImpVis Tutorial</iv-title-bar>
        <iv-visualisation>
            <center>
            <h1>ImpVis Components Documentation Library</h1>
            </center>

            <center>
            <div id="toc_container" >
                <center><h2 id="toc_title"><u>Contents</u></h2></center>
                <div id="left-column" style="display: inline-block; text-align:left;">
                    <h4 id="toc_cat">
                        <a  href="#layoutComponents">Layout Components</a>
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


                    <h4 id="toc_cat">
                        <a href="#buttonsAndInputs">Buttons and Inputs</a>
                    </h4>  

                    <ul>
                        <a href="#button">Button</a>
                    </ul>  
                    <ul>
                        <a href="#toggleAdvance">Toggle Advance</a>
                    </ul>  
                    <ul>
                        <a href="#toggleBasic">Toggle Basic</a>
                    </ul>
                    <ul>
                        <a href="#dropdownList">Dropdown List</a>
                    </ul>
                    <ul>
                        <a href="#dropdownTextbox">Dropdown Textbox</a>
                    </ul>
                    <ul>
                        <a href="#symbolButton">Symbol Button</a>
                    </ul>
                    <ul>
                        <a href="#slider">Slider</a>
                    </ul>
                    <ul>
                        <a href="#sliderBlock">Slider Block</a>
                    </ul>
                    <ul>
                        <a href="#tickbox">Tickbox</a>
                    </ul>
                    <ul>
                        <a href="#tabs">Tabs</a>
                    </ul>
                </div>

                <div id="right-column" style="display:inline-block; float:right; margin-left:10vw; margin-right: 10vw; text-align:left;">
                    <h4 id="toc_cat">
                        <a href="#visualBits">Visual Bits</a>
                    </h4>  
                    <ul>
                        <a href="#HoverText">Hover Text</a>
                    </ul>
                    <ul>
                        <a href="#loadingBar">Loading Bar</a>
                    </ul>
                    <ul>
                        <a href="#loadingSpinner">Loading Spinner</a>
                    </ul>
                    <ul>
                        <a href="#meter">Meter</a>
                    </ul>
                    <ul>
                        <a href="#navigation">Navigation</a>
                    </ul>
                    <ul>
                        <a href="sidebarText">Sidebar Text</a>
                    </ul>
                    <ul>
                        <a href="#Titles">Titles</a>
                    </ul>


                    <h4 id="toc_cat">
                        <a href="#Other">Other</a>
                    </h4> 
                    <ul>
                        <a href="#dragAndDrop">Drag and Drop</a>
                    </ul>
                    <ul>
                        <a href="#svgDragAndDrop">SVG Drag and Drop</a>
                    </ul>
                    <ul>
                        <a href="#legacyWrapper">Legacy Wrapper</a>
                    </ul>
                    <ul>
                        <a href="#equationBox">Equation Box</a>
                    </ul>
                </div>

            </div>
            </center>
            
            <div style="margin-left:5vw; width:90vw; word-wrap: break-word;">
                <hr id="layoutComponents">
                <h2>Layout Components</h2>

                <hr id="pane">
                <h4>Pane</h4>
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

                <hr id="sidebarContent">

                <h4>Sidebar Content</h4>
                Place inside pane component. Wraps text.
                <br>
                <img src="./assets/SidebarContent.png">
                <h5>Props</h5>
                Name: showPagination <br>
                Type: Bool <br>
                Default: "true" <br>
                Description: Shows "next" and "previous" buttons for multi-page visualisations.<br><br>

                <hr id="sidebarSection">
                <h4>Sidebar Section</h4>
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

                <hr id="fixedHotspot">
                <h4>Fixed Hotspot</h4>
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

                <hr id="toggleHotspot">
                <h4>Toggle Hotspot</h4>
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

                <hr id="buttonsAndInputs">

                <h2>Buttons and Inputs</h2>

                <hr id="button">

                <h4>Button </h4>
                    <mark>iv-button</mark>: A button component for general use.
                    <br>
                    <img src="./assets/button.png" alt="Button Component">

                    <h5>Props</h5>
                    Name: disabled <br>
                    Type: Bool <br>
                    Default: "false" <br>
                    Description: Greys out the button and prevents it from emitting events. <br><br>

                    <h5>Events</h5>
                    Name: mouseover <br>
                    Description: Emits this when mouse cursor enters the region of the button component. <br><br>

                    Name: mouseleave <br>
                    Description: Emits this when mouse cursor leaves the region of the button component. <br><br>

                    Name: click <br>
                    Description: Emits this when the mouse button is pressed and the cursor is over the button. <br><br>

                <hr id="toggleAdvance">

                <h4>Toggle Advance</h4>
                    A button that allows users to switch between multiple modes. It is possible to disable the toggle by setting the prop "toggleDisabled" to "true".
                    <br>
                    <img src="./assets/ToggleAdvanceMode1.png" alt="Toggle Advance in mode 1">
                    <img src="./assets/ToggleAdvanceMode3.png" alt="Toggle Advance in mode 3">
                    <img src="./assets/ToggleAdvanceDisabled.png" alt="Toggle Advance disabled">
                    <h5> Props </h5>
                    Name: modes <br>
                    Type: Array <br>
                    Required: true <br>
                    Default: ["Option 1", "Option 2", "Option 3"] <br>
                    Description: The array container for the toggle modes text <br><br>

                    Name: initialModeIndex <br>
                    Type: Number <br>
                    Default: 0 <br>
                    Description: Setting the initial toggle mode <br><br>

                    Name: toggleDisabled <br>
                    Type: Boolean <br>
                    Default: false <br>
                    Description: Disable the input <br><br>

                <hr id="toggleBasic">

                <h4>Toggle Basic</h4>
                    A button that allows users to switch between two modes. It is possible to disable the toggle by setting the prop "toggleDisabled" to "true".
                    <br>
                    <img src="./assets/ToggleBasicTrueMode.png" alt="Toggle Basic in true mode">
                    <img src="./assets/ToggleBasicFalseMode.png" alt="Toggle Basic in false mode">
                    <img src="./assets/ToggleBasicDisabled.png" alt="Toggle Basic disabled">
                    <h5> Props </h5>
                    Name:           initialMode <br>
                    Type:           Boolean <br>
                    Default:        true <br>
                    Description:    Setting the initial toggle boolean <br><br>

                    Name:           toggleDisabled <br>
                    Type:           Boolean <br>
                    Default:        false <br>
                    Description:    Disable the input <br><br>

                <hr id="dropdownList">

                <h4>Dropdown List</h4>
                    A button that allows users to select a mode from a display/hide list of modes. It is possible to disable the dropdown by setting the prop "dropdownDisabled" to "true".
                    <br>
                    <img src="./assets/DropdownListMode1.png" alt="Dropdown list in mode 1">
                    <img src="./assets/DropdownListSelectMode.png" alt="Dropdown list in select mode">
                    <img src="./assets/DropdownListMode2.png" alt="Dropdown list in mode 2">
                    <h5> Props </h5>
                    Name: dropdownItems <br>
                    Type: Array <br>
                    Required: true <br>
                    Default: ["Option 1", "Option 2", "Option 3"] <br>
                    Description: The array container for the dropdown list text <br><br>

                    Name: initialDropdownIndex <br>
                    Type: Number <br>
                    Default: 0 <br>
                    Description: Setting the initial dropdown mode <br><br>

                    Name: dropdownDisabled <br>
                    Type: Boolean <br>
                    Default: false <br>
                    Description: Disable the dropdown button <br><br>

                <hr id="dropdownTextbox">

                <h4>Dropdown Textbox</h4>
                    A button that allows users to display/hide a text box. It is possible to disable the dropdown by setting the prop "dropdownDisabled" to "true".
                    <br>
                    <img src="./assets/DropdownTextBoxShortText.png" alt="Dropdown textbox with sample text">
                    <h5> Props </h5>
                    Name: buttonText <br>
                    Type: String <br>
                    Default: "Click me" <br>
                    Description: The string for the button content <br><br>

                    Name: dropdownText <br>
                    Type: String <br>
                    Default: "Add text" <br>
                    Description: The string for the text box content <br><br>

                    Name: dropdownDisabled <br>
                    Type: Boolean <br>
                    Default: false <br>
                    Description: Disable the dropdown button <br><br>

                <hr id="symbolButton">

                <h4>Symbol Button</h4>
                    A button with changeable symbol for various purposes. Examples are play button, pause button and stop button.
                    <br>
                    <img src="./assets/SymbolButtonPlay.png" alt="Symbol button with 'play' shape">
                    <img src="./assets/SymbolButtonPause.png" alt="Symbol button with 'pause' shape">
                    <img src="./assets/SymbolButtonStop.png" alt="Symbol button with 'stop' shape">
                    <img src="./assets/SymbolButtonReset.png" alt="Symbol button with 'reset' shape">
                    <img src="./assets/SymbolButtonHelp.png" alt="Symbol button with 'help' shape">
                    <h5> Props </h5>
                    Name: size <br>
                    Type: String <br>
                    Default: "" <br>
                    Description: Controls the size of the button. Alternatives are "small" and "large". <br><br>

                    Name: symbol <br>
                    Type: String <br>
                    Description: Controls the shape of the symbol. Choices are "play", "pause", "stop", "reset" and "help". <br><br>
                
                <hr id="slider">

                <h4>Slider</h4>
                    A ranged slider that allows user to control variable.
                    <br>
                    <img src="./assets/Slider.png" alt="Blue slider">
                    <h5> Props </h5>
                    Name: min <br>
                    Type: Number <br>
                    Default: 0.0 <br>
                    Description: Sets the minimum value of the slider <br><br>

                    Name: max <br>
                    Type: Number <br>
                    Default: 100.0 <br>
                    Description: Sets the maximum value of the slider <br><br>

                    Name: step <br>
                    Type: Number <br>
                    Default: 10.0 <br>
                    Description: Sets the step size in the range of motion of the slider <br><br>

                    Name: init_val <br>
                    Type: Number <br>
                    Default: 50.0 <br>
                    Description: Sets the initial value of the slider <br><br>

                    Name: disabled <br>
                    Type: Boolean <br>
                    Default: false <br>
                    Description: Used to disable the slider so the value cannot be changed <br><br>

                    Name: sliderValue <br>
                    Type: Boolean <br>
                    Default: false <br>
                    Description: Used to display slider value adjacent to the slider <br><br>
                    
                    Name: bubble <br>
                    Type: Boolean <br>
                    Default: false <br>
                    Description: Used to display slider value as a bubble above the slider thumb, which follows the thumb <br><br>

                    Name: sliderButtons <br>
                    Type: Boolean <br>
                    Default: false <br>
                    Description: Used to display buttons to increase or decrease the slider value by a fixed amount <br><br>

                    Name: buttonInput <br>
                    Type: Boolean <br>
                    Default: false <br>
                    Description: Used to display input to vary the sliderButtons increase or decrease amount, applied to both equally <br><br>

                    Name: lineTick <br>
                    Type: Boolean <br>
                    Default: false <br>
                    Description: Used to display line slider ticks at each step <br><br>

                    Name: numTick <br>
                    Type: Boolean <br>
                    Default: true <br>
                    Description: Used to display value slider ticks at each step <br><br>

                    Name: playSlider <br>
                    Type: Boolean <br>
                    Default: false <br>
                    Description: Differnet mode of slider where slider buttons move to and from the previous and next frame <br><br>

                    Name: button_step_init <br>
                    Type: Number <br>
                    Default: 10.0 <br>
                    Description: Sets the value of the sliderButtons <br><br>

                    Name: tick_decimals <br>
                    Type: Number <br>
                    Default: 0 <br>
                    Description: Sets the number of decimal places for the numTick <br><br>

                <hr id="sliderBlock">

                <h4>Slider Block</h4>
                    The iv-slider-block is a wrapper for the iv-slider component. 
                    It takes the props of iv-slider and creates a stackable block which contains the slider.
                    An example is shown below.
                    <img src="./assets/SliderBlockExample.png" alt="Code snippet of slider block example">
                    <h5> Props </h5>
                    Name: bubble <br>
                    Type: Boolean <br>
                    Default: true <br>
                    Description: Display slider value as a bubble above the slider thumb <br><br>

                    Name: playSlider<br>
                    Type: Boolean<br>
                    Default: false<br>
                    Description: Differnet mode of slider where slider buttons move to and from the previous and next frame<br><br>

                    Name: min<br>
                    Type: Number<br>
                    Default: 0.0<br>
                    Description: Sets the minimum value of the slider <br><br>

                    Name: max<br>
                    Type: Number<br>
                    Default: 100.0<br>
                    Description: Sets the maximum value of the slider<br><br>

                    Name: step<br>
                    Type: Number<br>
                    Default: 10<br>
                    Description: Sets the step size of the slider <br><br>

                    Name: init_val<br>
                    Type: Number<br>
                    Default: 50.0<br>
                    Description: Sets the initial value of the slider thumb<br><br>

                    Name: tick_decimals<br>
                    Type: Number<br>
                    Default: 0<br>
                    Description: Sets the number of decimal places for the display value of the slider tick at each step <br><br>

                    Name: colorBlock<br>
                    Type: String<br>
                    Default: "green"<br>
                    Required: true<br>
                    Description: Sets the theme color for the entire block. Currently there are 9 options to choose from: navy, blue, teel, green, orange, tangerian, yellow, purple and berry <br><br>

                    Name: unit<br>
                    Type: String<br>
                    Default: "kg"<br>
                    Required: true<br>
                    Description: Sets the unit of the slider <br><br>

                    Name: sliderName<br>
                    Type: String<br>
                    Default: "Slider Name"<br>
                    Required: true<br>
                    Description: Sets the name for the slider <br><br>

                    Name: guidanceIdentifier<br>
                    Type: String<br>
                    Description: Sets a unique id that can be read by the guidance identifdier and return the corresponding guidance page<br><br>

                    Name:helpButtonActivated<br>
                    Type: Boolean<br>
                    Default: true<br>
                    Description: Display the help button<br><br>

                <hr id="tickbox">

                <h4>Tickbox</h4>
                    A boolean checkbox component that can be disabled by setting the prop "toggleDisabled" to "true".
                    <br>
                    <img src="./assets/bluetick.png" alt="A blue tick">
                    <img src="./assets/greytick.png" alt="A grey tick">
                    <h5> Props </h5>
                    Name:           initialMode <br>
                    Type:           Boolean <br>
                    Default:        true <br>
                    Description:    Setting the initial checkbox boolean <br><br>

                    Name:           toggleDisabled <br>
                    Type:           Boolean <br>
                    Default:        false <br>
                    Description:    Disable the checkbox <br><br>

                <hr id="tabs">

                <h4>Tabs</h4>
                    The iv-tabs component is the wrapper component of the iv-tab component. 
                    It takes in multiple tabs and wraps them into a list. 
                    The transition effect when switching between tabs wrapped by this component was imported from iv-toggle-advanced.
                    <br>
                    <h5> Props </h5>
                    There is no props for this component.
                    <img src="./assets/Tabs.png" alt="Example of tabs">
                    An example of using the tabs is shown below:
                    <img src="./assets/TabsUsage.png" alt="Example of tabs implementation">
                    Make sure that the iv-tab component is wrapped by the iv-tabs component.

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

iv-visualisation{
    width:100vw;
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


img {
    padding: 0;
    display: block;
    margin: 0 auto;
    max-height: 90%;
    max-width: 85%;
}

hr {
    width: 100%;
    margin-bottom: 15vh;
    margin-top: 10vh;
}

#toc_container {
    background: #f9f9f9 none repeat scroll 0 0;
    border: 1px solid #aaa;
    display: table;
    font-size: 95%;
    margin-bottom: 1em;
    padding: 20px;
    width: auto;
}

.toc_title {
    font-weight: 700;
    text-align: center;
}

.toc_cat {
    font-size: 13pt;
    line-height: 0.1em;
    border: 0px;
}

#toc_container li, #toc_container ul, #toc_container ul li{
    list-style: outside none none !important;
    font-size: 10pt;
    line-height: 0.4em;
}

mark {
    background-color:lightgray;
}

</style>



