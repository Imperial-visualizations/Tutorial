<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <center>
            <h1> An introduction to the development process. Part 2</h1>
            </center>
             <p>There have been purposefully no timelines included, as this will differ for each visualisation.</p>
             <p> The students are working on this project as an extracurricular activity.</p>
             <p> It is therefore important that there is no pressure for them to deliver during busy times - their academic work always has priority!</p>
             <p> Conversely, academic staff often work under substantial time pressure. We do not expect them to make themselves available at all times.</p>
            <p>Throughout the entire process, experienced staff and students are on hand to discuss and help develop the visualisations. </p>
            <p>Our community meets every Wednesday in term time from noon in our drop-in Code & Crisps sessions.</p>
            <p> These meetings are an excellent opportunity for staff and students to come in, have a chat, and have a go at developing your visualisation.</p> 
            <p>We hope that you will enjoy the process and that your final visualisations will prove to be of good use!</p>
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



