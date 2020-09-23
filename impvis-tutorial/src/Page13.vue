<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <center>
            <h1>Creating a branch</h1>
            </center>
            <p>When you're working on a project, you're going to have a bunch of different features or ideas in progress at any given time – some of 
                which are ready to go, and others which are not. Branching exists to help you manage this workflow.
                When you create a branch in your project, you're creating an environment where you can try out new ideas. 
                Changes you make on a branch don't affect the main branch, so you're free to experiment and commit changes, safe in
                 the knowledge that your branch won't be merged until it's ready to be reviewed by someone you're collaborating with.</p>
            <p>You ideally want to be working in a <b>branch</b> that is not <i>master</i> within your repository. You want to have 
            some working version of the code in master. You can build any experimental or new feature in a branch such as <i>dev</i> (for development).
            This divide means that you will always have a functional version of the visualization!</p>
            <img src="@/assets/images/gitkraken_branch_creation.png"  style="width:563px;height:300px;" align = "right"/>
            <p><b>Command:</b></p> To create a new branch (let’s call it <i>dev</i>) within your local repository, enter <code>git branch dev</code> into the
            terminal. Then, to move your working space into that branch, use <code>git checkout dev </code>.
            <p><b>Gitkraken:</b></p>To create a new branch within your local repository for development of code (using the same example of a 
            development branch), (in Gitkraken,) right-click on the ‘master’ branch from the ‘Local’ dropdown followed by ‘create a branch here.’
             Now you may name it ‘dev’,
             and start to develop the code. Again, it is better to work on the dev branch than the master branch.
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



