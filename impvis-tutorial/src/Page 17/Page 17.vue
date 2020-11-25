<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <div class="iv-main">
  <center>
            <h1>Common error messages and the way to handle them</h1>
            <redText>This section needs expanding on continually. If you learn something not on this page, please help by adding to it!</redText>
            </center>
            <p>If you commit to making changes to the same file or line of code as others, you may encounter a merge conflict.</p>
            <p><b>Commmand: </b><redText>Not sure, someone help!</redText></p>
            <p><b>GitKraken: </b>Note: Ideally, developers should work on independent files to avoid such situations.
For more details on git, please check out <a href = "https://rogerdudler.github.io/git-guide/">https://rogerdudler.github.io/git-guide/</a> or any other number of online resources on the basics of git.</p>
            
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
    name:"Page17",
}
</script>
<style>
.iv-main {
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
redText 
{ 
    color: red; 
} 

</style>



