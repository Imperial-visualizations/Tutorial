<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <center>
            <h1>Some help on HTML, CSS, JS and JS libraries (part 2)</h1>
            <h2>Cascading Style Sheet</h2>
            </center>
            <p>
                Cascading Style Sheet, or CSS, is how we style almost everything on a given web page. 
                CSS is a series of properties and their corresponding values describing all the stylistic 
                features of an HTML element. For example, the following piece of code can set the width, height, 
                and text colour of a div:
               0<center> <code>width:100%; height: 100%; colour: “#003E74”;</code></center>
            </p>
            <p>
                Everything from colour to size to animations is defined using CSS. One way of defining an HTML elements style 
                using CSS is to embed the CSS directly into the element. An example of embedding CSS directly in an HTML element is:
                <center><code>&lt;div class = “textbox” id = “theory” style = “width:100%; height: 100%; colour: “#003E74”;”&gt; Hello world! &lt;\div&gt;</code></center>
            </p>
            <p>
                <i>
                    Note: If you don’t understand the above code, it may be useful to look at the HTML section in the Functionality Guidelines document!
                </i>
            </p>
            <p>
                Alternatively, an element's style can be inherited from a class or ID, with the actual CSS written in a separate standalone 
                file. An example for the HTML in this case is: <code> &lt;div class = “textbox” id = “theory”&gt; Hello world! &lt;\div&gt;</code>
                With the separate stylesheet containing the following CSS:
                <ul>
                    <li><code>.textbox{</code></li>
                    <li><code>     width: 100%;</code></li>
                    <li><code>     height: 100%;</code></li>
                    <li><code>}</code></li>
                </ul>
                And
                <ul>
                    <li><code>#theory{</code></li>
                    <li><code>Colour: “#003E74”;</code></li>
                    <li><code>}</code></li>
                </ul>
            </p>
            <p>
                A typical visualisation will have a basic inherited style from one of two global stylesheets: skeleton.css and style.css. Any further detailed styling by a developer is typically done directly in the HTML file.
            For more on CSS, visit:
                W3 Schools: <a href="https://www.w3schools.com/css/css_intro.asp">https://www.w3schools.com/css/css_intro.asp</a>
            </p>
            <p>
                <b>Note on Sizes:</b>When defining a class's dimensions in a CSS file, this can be done using absolute or relative units. 
                Note that in the first line of example code in the document, relative units have been used (height and width defined in percent).
                 Another way of using relative units would be to write height in terms of "vh" (view height) and width in terms of "vw" (view width); 
                 e.g.:<code>width:75vw; height: 85vh;</code>. Here, 1vw means 1% of the width of the viewport (the user's visible area of a web page) 
                 and the same for vh.
            </p>
            <p>
                Absolute sizes are generally defined in pixels, e.g.:<code>width:550px; height: 300px;</code>. The disadvantage of this method of defining sizes is that certain elements will end up being different sizes, depending on the user's screen's resolution. For this reason, when defining div sizes, it is strongly recommended you use relative units.
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



