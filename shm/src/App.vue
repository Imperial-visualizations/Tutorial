<template>
    <div>
        <iv-title-bar>This is my title</iv-title-bar>
        <iv-visualisation>
            <template #hotspots>
                <iv-pane position="left">
                    Hi! This is a pane
                </iv-pane>

                <iv-toggle-hotspot position="bottom" title="Button Title"> 
                    <iv-slider @sliderChanged="slider1Change" :colorBlock="green" :max="0.02" :min="0.0005" :init_val="0.01" :sliderName="'slider test'" :unit="'test unit'" :step="0.0005" />
                    <iv-slider @sliderChanged="slider2Change" :colorBlock="green" :max="200" :min="1" :init_val="50" :sliderName="'slider test'" :unit="'test unit'" :step="1" />
                </iv-toggle-hotspot>
                
                <iv-fixed-hotspot position="topright" title="Fixed">
                    This will go inside the fixed hotspot, so will always appear on the screen.
                    P.S. You must specify a title and position.
                </iv-fixed-hotspot>

            </template>

            <MainStage v-bind:freq="slider1" v-bind:amp="slider2"></MainStage>

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
    props:{
        slider1: {
            default: 0.005,
        },
        slider2: {
            default: 50,
        }
    },
    methods:{
        slider1Change(e){
            this.slider1 = e;
        },
        slider2Change(e){
            this.slider2 = e;
        }
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



