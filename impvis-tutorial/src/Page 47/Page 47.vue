<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <div class="iv-main">
<center>
            <h1>4. Legacy (Content saved from old)</h1>
            <h2>jQuery</h2>
            </center>
            <p>
                jQuery is a JavaScript plugin that allows more effortless interactivity between the user and different 
                HTML elements. After importing jQuery in your HTML head, you can then treat any HTML elements as a pseudo-JS 
                variable. To do this, you can reference an element by id:
                <center><code>let Length = $(“#lengthslider”);</code></center>where the id is “lengthslider” in this case. Or by class:
                <center><code>let Length = $(“.slider”);</code></center>
                where the class is “slider” in this case. Generally, it is very good practice to use ID, <b>NOT</b> class, when specifying any one element.
            </p>
            <p>
                When a HTML element is defined in JS, jQuery can then call several different functions on that element. 
                One of the most important functions we use is the value function, which can either return the value of a HTML element:
                <center><code>let value_of_element = Length.val();</code></center>
                Or can set the value of the HTML element: <center><code>Length.val(“Hello Mars!”);</code></center>
            </p>
            <p>
                For more on jQuery, visit <a href="https://www.w3schools.com/jQuery/">https://www.w3schools.com/jQuery/</a>.
            </p>
            <center><h2>p5.js</h2></center>
            <p>
                p5.js is a drawing tool that allows developers to create non-plot graphics (such as a mass and spring) with heavy mouse 
                interactivity. It does this by repeatedly drawing objects on a canvas at a rate equal to 1/framerate. After p5 is imported 
                in your HTML header, the first step you will want to take is creating setup and draw functions in your JS file:
                <center><code>function setup() {let canvas = createCanvas(500,400);canvas.parent(‘canvas’);frameRate(60);};</code></center>
            </p>
            <p>
                <center><code>function draw() {clear();background('#ffffff');noStroke();fill("#A51900");rect(mouseX, mouseY, 75,75);};</code></center>
            </p>
            <p>P5 automatically recognises these two functions. Setup defines all the essential meta-variables for p5’s drawing, 
                variables such as frame rate and canvas size (specified in pixels). The Draw function is then carried out every 
                [1/framerate] seconds. Good practice for p5 is first to clear any previous drawings, then draw your background. 
                After that, you can draw your objects. In the example above, a brick red square is drawn at the mouse position with 
                length and width equal to 75px.
            </p>
            <p>
                For more on p5.JS visit <a href="https://p5js.org/.s">https://p5js.org/.s</a>
            </p>
            </div>
            
        </iv-visualisation>
    </div>
</template>
<script>
export default {
    name:"Page47",
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



