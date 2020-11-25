<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <div class="iv-main">
                <center>
            <h1>4 "while coding" a. Functionality guide</h1>
            <h2>Structuring Scripts</h2>
            </center>
            <p>
                As ImpVis is a learning place for everyone, we want them to understand our code too. 
                Most importantly is to have the code structured into blocks that are <b>maths</b>, <b>interaction</b>, and <b>calling</b>. 
            </p>
            <p>
                <b>Maths</b>-contains all the maths behind a visualisation. The output of this mathematical ‘black box’ should be data to be used in plotting.#
                <ol>
                    <li>Start by defining maths constants and variables—for example, the gravitational constant.</li>
                    <li>Then define maths functions and tools. For example, a function that returns the force on a mass-spring system.</li>
                </ol>
            </p>
            <p>
            <b>Interaction</b>-contains all non-mathematical functions.
            <ol>
                <li>Start by defining interaction constants and variables. For example, a mass slider can be defined as M = $(#mslider)</li>
                <li>Then define interactive functions, i.e., the functions that insert HTML values into math functions and insert the outputted data into plotting functions.</li>
            </ol>
            </p>
            <p><b>Calling</b>– specifies which functions are called in which instance.
                <ol>
                    <li>Specify which functions are called on the interaction of a jQuery element. For example, on “input.”</li>
                    <li>Specify which functions are called when the page is first loaded. </li>
                </ol>
            </p>
            <p>
                We want this structure as it allows people who perhaps don't understand the mathematics/theory 
                we're using to optimize the code without worry. It should work under the lines of "I have a set 
                of functions I've defined that when I input the user's input, I get the numerical values I need out" 
                before doing any plotting. The interaction code is then everything that's needed to get the JavaScript 
                and HTML files to talk to one another. It finds takes the user input (which is found through HTML), inputs 
                it into the maths block and takes the output, and puts it into any plots you want to have. Finally, the 
                calling section updates everything you need, so if the user has, for example, changed the value of some slider, 
                the calling section of the code will respond to this change and call a single function that does everything 
                you need to update the plots.
            </p>

            <p>
                Having the code ready in this general structure makes the work of those optimizing the code and checking 
                for redundancies much more comfortable, as it’s evident from the beginning what everything is doing. Provided 
                you’ve done the maths correctly; it allows those who don’t know the subject to do optimisation.
            </p>

            <p><i>
                Important Note: It is generally recommended that the same function, ‘Update()’ is called for both inputs and onload 
                of the page, with a variable called newpage, taking either a true or false value. This is because the only difference 
                between an onload and onclick function is whether to use the plotly.newplot() function or the plotly.animate() (or plotly.react()) 
                function. Everything else is the same.
            </i></p>
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
    name:"Page39",
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



