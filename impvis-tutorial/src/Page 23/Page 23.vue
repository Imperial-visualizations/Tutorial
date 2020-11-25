<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <div class="iv-main">
 <center>
            <h1>Creating Visualisations</h1>
            </center>
            <p>The best way to create visualisations is to use the create-impvistool, which automatically sets you 
            up with a project folder with a working template and git repository already set up! The create-impvis tool can be 
            installed once you have Node.js installed by using the Node Package Manager (NPM). To check that you have both of these programs 
            installed correctly on your computer, you will need to open a terminal window and run: <code>node -v && npm -v</code></p>
            <p>
            If Node.js and NPM are correctly installed on your system, you should see two version numbers printed (the exact number doesn't matter).
            With Node and NPM setup on your machine, you can install the CLI by running globally:
            <code>npm -g install @impvis/cli</code> and wait for the CLI to be downloaded and installed on your machine.
            </p>

            <center>
            <h1>Usage</h1>
            Creating Visualisations with the Vue CLI is a breeze! To create a visualisation, open a new terminal window in the directory
            you wish to create the visualisation folder. Then run: <code>impvis create <i>name</i></code>
            </center>
            <p>Where <i>name</i> is the name of your visualisation (decide that here). You will then be guided through step by step prompts 
            to allow you to configure the base visualisation template to suit your needs. At present, the CLI has four template options available 
            for users to choose from:</p>
            <ol>
                <li>Current template using Node.js</li>
                <li>Current template using a &lt;script&gt; import</li>
                <li>Basic legacy template from Summer 2019</li>
                <li>Advanced legacy template from Summer 2019</li>
            </ol>
            If you're new to ImpVis, we recomment the first option.
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
    name:"Page23",
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



