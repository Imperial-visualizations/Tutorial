<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <div class="iv-main">
   <center>
            <h1>Adding SHM to the pane</h1>
            </center>
            <p>Firstly, if you want to copy and paste this code, check out the shm folder contained in the GitHub repository for this
            tutorial document at <a href = "https://github.com/Imperial-visualizations/Tutorial">https://github.com/Imperial-visualizations/Tutorial</a>. 
            This document is intended to be useful behind seeing the logic of setting up such a visualisation, as opposed to providing the code to be changed.
            But please do spend some time messing around with it!</p>
            <p>The code to produce an object which performs SHM is pasted to the left of this text. This should sit in the MainStage.vue file, as we 
                want to treat the SHM block as a component, which we can use multiple times anywhere. 
            <img src="@/assets/images/shm_code.png"  style="width:495px;height:990px;" align = "left"/>
            Specifically, the code makes a basic SHM vis using a prop for any variables I may want to control with sliders/buttons. When you run this code,
            you should see a ball conducting SHM on the screen. 
            </p>
            <p>
                Sliders which control the SHM motion can be be added, to see this in action, check out the App.vue file in the SHM vis, from there, you will 
                be able to see how interaction with the MainStage component is brought about.
            </p>
            </div>
         
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
    name:"Page31",
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



</style>



