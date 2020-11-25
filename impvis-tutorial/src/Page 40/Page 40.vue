<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <div class="iv-main">
 <center>
            <h1>Some help on HTML, CSS, JS and JS libraries</h1>
            <h2>HTML</h2>
            </center>
            <p>HTML is less of a language and more of a collection of blocks or ‘elements’ that define what goes on your page. 
                These elements are defined using opening and closing tags. For example, if I wanted to have an element displaying 
                “hello world,” I would have an open <code>&lt;div&gt;</code> tag, followed by the text, followed by a closing <code>&lt;/div&gt;</code> tag. So overall, 
                the element looks like:</p>
                <center><code>&lt;div&gt;hello world&lt;/div&gt;</code></center>
            <p>When constructing your own HTML, it is likely to be composed of two sections: a head and a body. In the Head, 
                all of your external packages apart from your JavaScript file(s).  For example, if I were using MathJax to write my 
                equations, I would put the MathJax importing script into the Head. The body contains the actual elements that appear 
                on the page. Then, you should import your JavaScript (or JS) files at the end of the body. This is done because if the 
                JS files were in the Head, they might reference things that aren’t defined yet.
            </p>
            <p>
                For more tutorials on HTML, here are a few useful resources:
                <ul>
                    <li>W3 Schools: <a href="https://www.w3schools.com/html/html_intro.asp">https://www.w3schools.com/html/html_intro.asp</a></li>
                    <li>CodeAcademy: <a href="https://www.codecademy.com/learn/learn-html<">https://www.codecademy.com/learn/learn-html</a></li>
                </ul>
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
    name:"Page40",
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



