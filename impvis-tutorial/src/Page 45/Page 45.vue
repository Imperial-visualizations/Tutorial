<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <div class="iv-main">
  <center>
            <h1>Debugging and Console</h1>
            <span class="red">This page should be continually expanded upon, if you can add something to this page, please do!</span>
            </center>
            <p>In Python, debugging is easy - you press play, and if there is an error in the code, your interpreter tells you precisely what 
                and where it is. For web development, debugging is a little trickier, but the golden rule is F12 (or fn+F12 for some keyboards) 
                is your best friend! This hotkey (or right-click + inspect for mac) brings up the browser developer tools, composed of several 
                tabs. Of these, the <i>elements</i> tab is essentially your HTML/CSS debugger. If you hover over the HTML brought up in this tab, 
                the div will be highlighted on the actual web page. Here we can see the div and its corresponding padding highlighted on the page 
                when the <i>container</i> div is hovered over:
                <center><img src="@/assets/images/console.png"  style="width:690px;height:459x;" align = "down"/></center>
            </p>
            <p>
                The second important tab to know about is the console tab. This is essentially your JavaScript debugger. Any error reports in your JS code will pop up here in red, and if you click on the error, it should take you to the JS code where the error was found. Also, the analogy to the python print(“hello world”) in JS is console.log(“hello world”), where the printed output should appear in the console tab. However, when you have finished your debugging, it is very important to remove all console.log commands, so they do not stay in your page's live version!
            </p>
            </div>
          
        </iv-visualisation>
    </div>
</template>
<script>
export default {
    name:"Page45",
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
.red{
    color:red;
}

</style>



