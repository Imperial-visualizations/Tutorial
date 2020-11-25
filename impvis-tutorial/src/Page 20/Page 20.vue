<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <div class="iv-main">
  <center>
            <h1>2. Setting up the coding environment</h1>
            <h2>2a. The Languages </h2>
            </center>
            <p>
                Hypertext Markup Language (HTML) is the backbone of any webpage, and this is the case for Imperial Visualisations. HTML is less of a language and more of a collection of blocks or ‘elements’ that define what goes on your page. HTML allows us to define everything on our page, but cannot do much else. For the most part, HTML is static and cannot perform complex equations or plotting. This is where JavaScript (JS) comes in. Imperial Visualisations uses JS to perform physical/mathematical calculations, plot, and achieve interactivity. These elements can contain anything from text to a slider to a graph plot, and can be styled to your preference! From the size of your element to the text color, this styling can all be specified using another language: Cascading Style Sheet (CSS). 
            </p>
            <p>
                Here are a few Links to relevant places on how to do some basic HTML, CSS and JS -
                <ul>
                    <li><b>HTML</b>: <a href="https://www.codecademy.com/learn/learn-html">https://www.codecademy.com/learn/learn-html</a></li>
                    <li><b>CSS</b>: <a href="https://www.codecademy.com/learn/learn-css">https://www.codecademy.com/learn/learn-css</a></li>
                    <li><b>JS</b>: <a href="https://www.codecademy.com/learn/introduction-to-javascript">https://www.codecademy.com/learn/introduction-to-javascript</a></li>
                </ul>
            </p>
            <p>
                For the HTML course, you will most likely require sections 1. <i>Elements and Structure</i>, and 3. <i>Forms</i>.
                You may choose to opt-out on learning CSS as we have a set of predefined components, like sliders and buttons, which will be introduced later! If you are interested in customising the components, you may come back and learn CSS.
                As for JS, sections 2-7 are essential, and sections 8 and 9 are useful for object-oriented programming.
            </p>
            <p>
                While coding a visualisation, you will inevitably have to use some mathematical functions. <i>Math.js</i> is an extensive JS math library that provides many useful tools. For more information, <a href="https://mathjs.org/">https://mathjs.org/</a>.
            </p>
            <p>
                ***From here, we will assume knowledge of basic HTML and JS.***
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
    name:"Page20",
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



