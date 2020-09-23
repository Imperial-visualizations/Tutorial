<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <center>
            <h1>4b. The ImpVis Visual Identity -  Text</h1>
            </center>
            Imperial College London’s executive typeface “Meta normal” is used as the font on all visualisations. For more information on this, see:
            <a href="https://www.imperial.ac.uk/brand-style-guide/visual-identity/font/">https://www.imperial.ac.uk/brand-style-guide/visual-identity/font/</a>
            You can refer to “Notes_on_format_for_clarity_and_comprehension.pdf” in this repository for more details.
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



