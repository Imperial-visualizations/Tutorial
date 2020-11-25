<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <center>
            <h1>Extra comments for the developer</h1>
            </center>
            <h2>Git Ignore node_modules</h2>
            <p>
                To share your projects more easily, you should exclude the node_modules folder from your github repo. 
                Otherwise people will get an error when they run <code>npm run serve</code> which can be solved by deleting the node_modules 
                folder and running <code>npm i</code>. 
            </p>
            <p>
                To exclude the node_modules folder you must create a .gitignore file in the project directory.
                <ol>
                    <li>In your main project directory (the folder containing the node_modules folder) create a file and name it “gitignore.txt”.</li>
                    <li>Open this in a text editor and add the following text “node_modules/” then save and close the file.</li>
                    <li>Hold shift and right click in the project folder and click “open terminal here” or “open powershell here”.</li>
                    <li>Run this command <code>ren gitignore.txt .gitignore</code></li>
                    <li>Then run this command <code>git rm -r --cached node_modules/</code></li>
                    <li>Then using gitkraken or command line git, commit and push your changes. </li>
                </ol>
                You should now retain your version of the “node_modules” folder, but your git should not have any “node_modules” folder. 
                Now other people can clone the repo and just run the command <code>npm i</code> then <code>npm run serve</code>.
            </p>
            <h2>NPM node modules</h2>
            <p>
                Do not edit the vue-components files in node modules. Instead if something isn't working you need to clone the 
                vue-components repository, and then edit that to make your visualization work, then pull request the changes you’ve 
                made to the vue components repository.
            </p>
            <h2>YouTube videos for the developer: </h2>
            <p>Check out the channel <a href=" https://www.youtube.com/channel/UCCWiTDeqBPSsUks0jFrhEKQ"> https://www.youtube.com/channel/UCCWiTDeqBPSsUks0jFrhEKQ</a></p>
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
    name:"Page50",
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



