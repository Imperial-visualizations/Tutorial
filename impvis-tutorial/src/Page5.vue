<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
             <template #hotspots>
                <iv-pane position="left" width ="450">
                    <img src="@/assets/images/Development_cycle.png"  style="width:400px;height:500px;"/>
                    <br>The development cycle.
                </iv-pane>
            </template>
            <center>
            <h1> An introduction to the development process</h1>
            <i>An overview of the process of going from the initial idea to implementing it: </i>
            </center>
            <p>Outlined below are the six essential steps of the development process. Full descriptions and guides to completing each section are given later in this document.</p>
            <ol>
            <li>Connect with our community! We use <b>Slack</b> for team communication, <b>Trello</b> for keeping track of visualisations in development, and <b>Github</b> for sharing code.</li>
            <li>During this phase, students will start developing the many new skills required to develop visualisations, such as code-sharing on <b>Github</b> and programming in <b>Javascript / HTML / CSS</b>.</li>
            <li>Before any coding starts, there needs to be a clear plan for ‘version 1.0’ of the visualisation; this requires defining <b>learning objectives</b> and creating a <b>design sketch</b>.</li>
            <li> This step is the <b>programming</b> phase. With the aid of a visualisation template the student(s) will code up the ‘version 1.0’ functionality in Javascript / HTML / CSS.</li>
            <li> Once all the functionality has been coded up, the visualisation is sent for <b>peer-review</b>, leading to further improvement and development before sending it for <b>staff review</b>.</li>
            <li>After checking ‘version 1.0’ for correctness, the staff partner <b>approves</b> the visualisation. It will then be <b>uploaded</b> to the website. Optional extensions can initiate a new design phase.</li>
            </ol>
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
</style>