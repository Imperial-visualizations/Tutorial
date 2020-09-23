<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <h1>Step 3: Cloning a repository (in Gitkraken)</h1>#
            GitKraken: To clone a repository to a location, you need two things: 
            a repository to clone, and a location to clone it to. First, choose a 
            repository to clone by going to<a href="https://github.com/Imperial-visualizations"> https://github.com/Imperial-visualizations</a> and
            selecting a repository (by clicking on one of the prominent blue hyperlinks),
            for example, Lattice-Vibrations. Once you have opened the repository location on GitHub,
            you can copy the location. Do this either by copying the URL at the top of the screen or by
            clicking the green “code” button, followed by the copy icon (grey button).<br>
            <img src="@/assets/images/cloning.png"  style="width:602px;height:300px;" align = "left"/><br>
            Once you have copied the repository location, open GitKraken, once you have, click (on the top left of the screen) on “File” > “Clone Repo.”
            “Clone with URL” should already be selected, but if it is not, select that. Then, paste the repository location into the URL entry as here: 
            <center><img src="@/assets/images/filepath_gitkraken.png"  style="width:401px;height:217px;"/></center>
            (using the Lattice-Vibrations repo as an example again: <a href="https://github.com/Imperial-visualizations"> https://github.com/Imperial-visualizations</a>).
            The steps above are everything needed to link up the repository location correctly. Now you have to select a location to clone this repository to. To do this, 
            click on Browse, go to the location you want to store these files (perhaps create a new file), click open older, and finally "Clone the repo!".
             Once you've made the clone, you can open the repository. Do this by clicking "Open now" when it is finished cloning, or later by clicking on "File">
              "Open Repo," and select the folder that you cloned the repository to.

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
  padding-top: 0px;
  padding-bottom: 50px;
}

code {
    background-color: #eee;
    border-radius: 3px;
    font-family: courier, monospace;
    padding: 0 3px;
}

</style>



