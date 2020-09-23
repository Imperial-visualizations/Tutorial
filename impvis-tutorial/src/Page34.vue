<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <center>
            <h1>4 b. The ImpVis Visual Identity - Ethos</h1>
            </center>
            <p>
                At Imperial visualisations, we have several design principles and goals that 
                help guide how visualisations look and feel. As developers, you should always 
                keep these principles in mind; as long as you adhere to our ethos, your specific 
                styling can vary however you want.
            </p>
            <ul>
                <li><b>Playful</b>We want to encourage people to get involved in our visualisations. The colours, layout, and animation should be enticing and invite creativity and curiosity. </li>
                <li><b>Intuitive:</b>Although every ‘learn’ visualisation should be accompanied by guidance, any person should immediately interact with a visualisation. Buttons to be pressed and sliders to be dragged should seem to “pop” out the screen. 
</li>
                <li><b>Light:</b>In terms of tone, any Imperial Visualisation should never feel dark, heavy, or too artificial. Instead, it should feel light, fun, and natural.</li>
                <li><b>Clean and Concise</b> As we are dealing with difficult scientific concepts, one of our main priorities is not to overwhelm the user with complexity. As such, each visualisation should look clean and organised (but not disparate).
</li>
                <li><b>Part of a journey (for suites)</b>Every visualisation should be taking the user on a journey. The page's overall design should reflect this; the user’s attention should be drawn to the start of the visualisation journey and move slowly towards the journey’s end.
</li>
            </ul>
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



