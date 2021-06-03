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
                <h4>
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
            
            <div style="margin-left: 5vw;">
                <h2 id="layoutComponents">Layout Components</h2>
                <h4 id="pane">Pane</h4>
                <h4 id="pane">Pane</h4>

                <h2 id="buttonsAndInputs">Buttons and Inputs</h2>

                <h4 id="button">Button</h4>
                    
                <h4 id="toggleAdvance">Toggle Advance</h4>
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

                <h4 id="toggleBasic">Toggle Basic</h4>
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

                <h4 id="dropdownList">Dropdown List</h4>
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

                <h4 id="dropdownTextbox">Dropdown Textbox</h4>
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

                <h4 id="symbolButton">Symbol Button</h4>
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

                <h4 id="slider">Slider</h4>
                <h4 id="sliderBlock">Slider Block</h4>
                <h4 id="tickbox">Tickbox</h4>
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

                <h4 id="tabs">Tabs</h4>

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



