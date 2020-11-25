<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <div class="iv-main">
<center>
            <h1>Some help on HTML, CSS, JS and JS libraries (part 3)</h1>
            <h2>JavaScript</h2>
            </center>
            <p>
                For the most part, JS is structurally similar to python; it has functions that take input 
                variables equal to a String, Float, Integer, or Boolean. However, if you are coming from a 
                Python background, there are a few significant differences to note:
                <ul>
                    <li>Defining variables for the first time needs to be preceded with either <b>Let</b>, <b>Var</b>, or <b>Const</b>. For example, the start of your JS code could say const g = 9.8. The difference between these variable declarations is:</li>
                    <li>
                        <ul>
                            <li><b>Let</b> exists in a block-scoped namespace. I.e., if it is defined in a function, then it stays in that function.</li>
                            <li><b>Var</b> is very wishy-washy. Please do not use it.</li>
                            <li><b>Const</b> is also block-scoped, but cannot be reassigned.</li>
                        </ul>
                    </li>
                    <li>Rather than using indentation to define where a for loop/function is, JS uses curly brackets. For example:
                        <ul>
                            <li>This function returns the square of the input value:<code>function square(x) {return(x*x);}; </code></li>
                            <li>This for loop counts from 1 to 10:<code> for (let i=0;  i&lt;10; i++ {console.log(i);};</code></li>
                            <li>This if statement prints ‘yay’ if happy is true and ‘aww’ if happy is false:<code>if(happy===true){console.log(“yay”)}else{console.log(“aww”)};    </code></li>
                        </ul>
                        Note that although you don't need indentation to write JavaScript code, you are able to indent it however you like. Consistent
                    </li>
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
    name:"Page42",
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



