<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <center>
            <h1>Command vs. Gitkraken</h1>
            </center>
            <p>Now that you have an account, you can clone the repository (copy it to your local computer), make changes, and upload them to GitHub so that your changes get updated.There are two classic ways that we do this at Imperial Visualisations. One way is using command, and the other is using GitKraken.Command and GitKraken are equivalent methods to allow communications between your machine and our GitHub. Command (or Terminal) uses line commands, while GitKraken is an app that has all the equivalent actions.</p>
            <p>Both have their pros and cons; for example, GitKraken is more visual, has a shallower learning curve, and less to remember to use it. On the other hand, command works much faster and is more straightforward to fix the level of issues dealt with in code & crisps. If you continue programming in the future, you will most likely need to know how to use command eventually. You also look more like a hacker when using command. For further information about the benefits of using Gitkraken and Command, check out this comparison (by GitKraken...) https://support.gitkraken.com/pdf/infographic/gitkraken-vs-cli.pdf.                We do not have a preference for which one of these you use, half of us recommend using Command, the other half Gitkraken. The choice is yours!</p>
            <p>Once you have chosen, there are a few steps that you need to go through in order to make changes to files on GitHub. Here are some instructions on how to each step necessary to create and make changes to files you want on GitHub.</p>
            <center>
            <h1>Step 1: Downloading the service</h1>
            </center>
            <b>Command:</b> Congratulations, you already did - this is built in as Command Prompt on Windows or Terminal on MacOS.<br>
            <b>GitKraken:</b> To download GitKraken, please visit https://www.gitkraken.com/download and download it to a location you will remember.
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
  padding-top: 0px;
  padding-bottom: 50px;
}
</style>



