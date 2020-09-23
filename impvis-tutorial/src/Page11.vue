<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
        <h1>Step 3: Cloning a repository (in command)</h1>
            <p>In order to access the desired repository, we must clone it onto your local computer.
            To clone a REPOSITORY owned by USERNAME, use <code> git clone https://github.com/USERNAME/REPOSITORY</code>
            (Note, press enter to execute commands). For example, if I wanted to clone a repository such as “Lattice-Vibrations” I would do the following:
            </p>
            <ol>
                <li>Create a folder on my computer with which I would like to clone the repository e.g., <i>ImpVis_projects</i></li>
                <li>Then in the command line navigate to the folder you just created.</li>
            </ol>
            <p>Note, to navigate in command, Use  cd <i>directory</i> to navigate into a folder from the current folder you’re in. If you make a mistake, use <code>cd ..</code>
            To navigate to your root directory, use <code>cd /</code>
            An example: For me, the writer, say I wanted to reach my “Lattice Vibrations” folder in command, and say the root to that folder was 
                from the C drive which contained a folder “Visualizations”, which contained the “Lattice Vibrations folder”, then I’d use:
                1.) <code>cd /</code> to get back to the C drive. 2.) <code>cd Visualizations</code> to open “Visualizations”, then 3.) 
                <code>cd Lattice-Vibrations </code>to get into the “Lattice-Vibrations” folder. In Command, that would look something like </p>
                <img src="@/assets/images/cd-ing.png"  style="width:737px;height:125px;" align = "left"/>At this point, command is “in” the Lattice-Vibrations folder, 
                and is ready to carry out commands from there.<p>If you’d like further advice on how to navigate in command, check out https://www.git-tower.com/blog/command-line-cheat-sheet/</p>
            <p>Once you’ve opened the file you created earlier, enter <code>git clone https://github.com/Imperial-visualizations/Lattice-Vibrations.
                git</code>. Now that you have a local repository! You can now look at the code of the visualization in an IDE of your choice (most of us use VSCode).</p>
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



