<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <center>
            <h1> Opportunities to join</h1>
            </center>
            Weekly Code & Crisps sessions:
            <ol>
                <li>Open to anyone.</li>
                <li>Can work on any course / visualisation.</li>
                <li>We will help create a staff-student partnership.</li>
                <li>No pressure!</li>
            </ol>
            Summer team:
            <ol>
                <li>Will need to send an application.</li>
                <li>Specific targets will be set each summer.</li>
                <li>Supported by a weekly bursary from Student Shapers.https://www.imperial.ac.uk/students/studentshapers/</li>
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



