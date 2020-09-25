<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <div class="iv-main">
 <center>
            <h1>2b. The Software - Visual Studio Code</h1>
            </center>
            <p><img src="@/assets/images/vscode_welcome.png"  style="width:512px;height:289x;" align = "right"/><b>Download:</b>
             Visual Studio Code (VSCode) is the integrated development environment that we recommend. Still, you are free to use 
             any code editor that supports JS and HTML. To download VSCode, please visit <a href="https://code.visualstudio.com/download">
             https://code.visualstudio.com/download</a>. After installing and opening it, you should find this as your welcome page (right). 
            </p>
            <p><b>Creating a basic HTML and opening a folder in VSCode: </b>On the top left, click on File > New File, and you should 
            get an empty file called Untitled-1. Include the code in the following example and save it as <i>some_name.html</i>.
            <img src="@/assets/images/Hello_world.png"  style="width:512px;height:290x;"/>
            Now, open the file in a web browser (e.g., Google Chrome), you should see the the stuff on the image to the right:
             <img src="@/assets/images/Hello_world_display.png"  style="width:512px;height:66x;" align="right"><br>
             If you have created a folder for your HTML, you may want to open the VS Code folder. You can do it by dragging the folder into the Explorer:</p><img src="@/assets/images/vscode_folders.png"  style="width:159px;height512x;" align="left"/>

            </div>
        </iv-visualisation>
    </div>
</template>
<script>
export default {
    name:"Page21",
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



