<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <center>
            <h1>Making a repository</h1>
            </center>
            <p>At some point, you may want to write your own independent vis or suite in a new repository. As part of the work for the ImpVis website, this repository must be created on the ImpVis repository.</p>
           <p><b>Command[not actually using command line just github]:</b>
           <img src="@/assets/images/repository_creation.png"  style="width:330px;height:293x;" align = "right"/>
           <ol>
               <li>Go to <a href="https://github.com/Imperial-visualizations">https://github.com/Imperial-visualizations</a></li>
               <li>Click New(green button near top right)</li>
               <li>Enter the details of the new repository, name, etc. Make sure to make the repository public so that other developers can access your code! That’s it. You can now clone the repository and start working on your project.</li>
           </ol>   
           </p>
           <p><b>GitKraken:</b> Click on File > Init Repo > GitHub.com and change the account to imperial-visualizations (you need to have the developer’s permission). You may fill in the desired name, description, and ‘where to clone to’ on your machine. Please note that the access must be public as ImpVis is an open-sourced website. Once you have clicked ‘Create Repository and Clone’, you may open the cloned repository and use it.</p>
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



