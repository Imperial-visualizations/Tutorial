<template>
    <div>
        <iv-title-bar>This is my title</iv-title-bar>
        <iv-visualisation>
            <template #hotspots>
                <iv-pane position="left">
                    Hi! This is a pane
                </iv-pane>
                <iv-toggle-hotspot position="bottom" title="Button Title"> 
                    This will go inside the pop-out section
                </iv-toggle-hotspot>
                
                <iv-fixed-hotspot position="topright" title="Fixed">
                    This will go inside the fixed hotspot, so will always appear on the screen.
                    P.S. You must specify a title and position.
                </iv-fixed-hotspot>

            </template>

            <MainStage></MainStage>

        </iv-visualisation>
    </div>
</template>
<script>
import {name} from '../package.json';
import MainStage from './components/MainStage.vue';

export default {
    name:"App",
    components:{
        MainStage,
    },
    data(){
        return {
            projectName: name
        }
    },
}
</script>
<style>
.iv-welcome-message{
    display:flex;
    flex-direction: column;
    align-items: center;
    margin-top: 50px;
}
</style>



