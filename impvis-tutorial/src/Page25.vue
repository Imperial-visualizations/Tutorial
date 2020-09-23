<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <center>
            <h1>Current Template using <i>script</i> tag</h1>
            </center>
            <p>This template is recommended for people new to or just getting started with Vue.js. 
                It removes some of the additional complexity associated with a Node.js backend. 
                In this template, you work entirely within a single .html file with Vue and the 
                Imperial Visualisations library included with standard script tags located in the header.
            </p>
            <center><h2>Installing additional packages</h2></center>
            <p>
                Installing additional packages for this template is not as convenient as using the Node template 
                however is still relatively simple. The <i>UNPKG</i> repository can quickly retrieve a valid URL 
                for any library located on NPM. Additional dependencies can be added to the head section of the HTML file by writing:
                <code>&lt; script defer src="https://unpkg.com/&lt;my-package-name&gt;/@version-number </code>

            </p>
            <p>
                You may need to read the library documentation you are importing to see if there are any additional 
                files such as CSS files that also need to be imported.
            </p>
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



