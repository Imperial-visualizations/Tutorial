<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <center>
            <h1>4 review a. The Writer and Peers</h1>
            </center>
            <p>
                Any particular visualisation must be reviewed before it is incorporated into the website. This keeps 
                up the quality of the content! Here is a set of questions a vis writer can ask as an initial review:
                <ol>
                    <li>Has the vis achieved the primary learning outcome?</li>
                    <li>Is the vis physically correct or at least visually giving the right intuition?</li>
                    <li>Is it intuitive to use?</li>
                </ol>
                And for a suite:
                <ol>
                    <li>Has the suite achieved secondary learning outcomes?</li>
                    <li>Does every vis work correctly/the way you want?</li>
                    <li>Does it flow?</li>
                    <li>Is it easy to follow through?</li>
                </ol>
                (Bug check: Have you looked into exceptional cases if they exist?)
            </p>
            <p>
            At this point, it’s best if you can get someone with “clean eyes,” either someone who has not seen the subject 
            you’re trying to teach yet or someone who has not seen your visualization trying to teach the content you’re doing. 
            Peers are an excellent choice! This peer review gives you feedback on how easy it is to understand what’s been said.
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



