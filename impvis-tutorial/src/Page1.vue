<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <center>
            <img src="@/assets/images/ImpVis-logo.png"/>
            
            <h1> Welcome to the ImpVis tutorial</h1>
            This is a document that aims to tell you everything you need to know, from start to finish, when creating a visualisation.<br> Check out the ImpVis website by clicking on the logo
            on the top right of the page.<br> 
            Please note, if you have any further questions, feel free to get in touch with Caroline Clewley at c.clewley@imperial.ac.uk
        </center>
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
</style>



