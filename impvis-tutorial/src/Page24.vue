<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <center>
            <h1>Current Template using Node.js</h1>
            </center>
            <p>This template is the <b>recommended</b> template for all new projects from now on as it 
            comes with a pre-configured node.js instance, which makes running automated tasks, 
            linting your code for errors, and optimising your code for all browsers a breeze. 
            It also includes the Imperial Visualisations Vue Components library as standard, 
            already set up and ready to go! Using this template, you will create visualisations 
            using the Vue Single File Component files <i>(.vue)</i>, which allows you to divide your 
            visualisation up into <b>sub-components</b>, each containing all the HTML, JS, and CSS needed 
            for the component to function correctly. For a refresher on how components work, you 
            should check out the <i><a href="https://www.youtube.com/watch?v=EpOEOPPAtWw>">Introduction to Components</a></i> video on the ImpVis Youtube channel.
            </p>
            <center><h2>Installing additional packages</h2></center>
            <p>Using this template, it is easy to install additional modules after the fact simply by running:
            <code> npm install <i>my-package-name</i></code>, where <i>my-package-name</i> is the name of the package
            containing the modules you want to install. This automatically downloads and installs the relevant package from the NPM repository.
            You can then use ES6 import statements to access the features of the library.</p>
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



