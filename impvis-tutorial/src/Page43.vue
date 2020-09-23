<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <center>
            <h1>Some help on HTML, CSS, JS and JS libraries (part 4)</h1>
            <h2>Plotly</h2>
            </center>
            <p>
                Plotly is a plotting package based on the D3 library. Most interactive plots in our visualisations have been made using Plotly, due to its simplicity and great style right out of the box. After including Plotly in your HTML head, you will mostly be dealing with Plotly through three functions:
                <ul>
                    <li><code>plotly.newplot(graph_id,data,layout)</code></li>
                    <li>This function creates a plot in a previously unoccupied div with id graph_id. The data and layout inputs define what data is plotted and how the plot looks. Use this to initialise your plot.</li>
                </ul>
            </p>
            <p>
                <ul>
                    <li><code>plotly.animate(graph_id, frames,animation_attributes)</code></li>
                    <li>This function updates the data of an already existing plot in the element with id = graph_id. The frame variable defines the new set of data. Use this for animating a constant set of points or a line, for example.</li>
                </ul>
            </p>
            <p>
                <ul>
                    <li><code>plotly.react(graph_id, data, layout)</code></li>
                    <li>This function updates both the data and layout of an existing plot with id=graph_id. Use this if you need to animate axis sizes, for example, or if your new data set has different dimensions to the old one.</li>
                    <li></li>
                </ul>
            Notice how in all three functions, there is either a <b>data</b> or <b>layout</b> variable (or both). These are the two most essential variables in Plotly, and have a basic dictionary-like structure that is super intuitive! Let’s take a look at a <b>data</b> example first:
            <ul>
                <li><code>var data=[{type:"scatter",mode:"lines",x: [0,2,5,7,3],y: [1,6,3,7,8],line:{color:"#960078", width:3, dash: "dashed"},         },];</code></li>
            </ul>
            As you can see, data is a list of dictionaries, where the dictionaries’ entries are properties of a dataset, properties such as x, y, and data label. Data is a list because Plotly allows for the addition of multiple datasets at once onto a plot.
            </p>
            <p>
            Now let’s look at a <b>layout</b> example:
            <ul>
                <li><code>const layout = {autosize: true,margin: {l:30, r:30, t:30, b:30},hovermode: "closest",showlegend: false,xaxis: {range: [-10,10], zeroline: true, title: "x"},yaxis: {range: [-10,10], zeroline: true, title: "y"},aspectratio: {x:1, y:1}};</code></li>
            </ul>
            As you can see, the layout is a single dictionary defining stylistic features of the plot, such as its size and margins. For more on how you should style a Plotly graph, visit the style guidelines page. For more on Plotly, the two most important resources are:
            <ol>
                <li><b>Function reference</b> - <a href="https://plot.ly/javascript/plotlyjs-function-reference/">https://plot.ly/javascript/plotlyjs-function-reference/</a></li>
                <li><b>Full reference</b> -<a href ="https://plot.ly/javascript/reference/">https://plot.ly/javascript/reference/</a></li>
            </ol>
            </p>
            <p>
                <center><i>Important note: Plotly can often be the reason a given page is slow or unoptimized. Look out for slow ways of updating a graph, such as plotly.purge() and plotly.newplot().</i></center>
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



