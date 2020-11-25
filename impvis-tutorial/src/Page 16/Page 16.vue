<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <div class="iv-main"><center>
            <h1>Merging the branches</h1>
            </center>
            <p>Let’s say that you have done a few commits and have a version of your vis that you are ready 
                for a milestone saving of all the commits; you can merge the dev branch into master.
            </p>
            <p><b>Command:</b> If I wanted to merge in my experimental code, which I have now thoroughly tested from the 
            <i>dev</i> branch into the <i>master</i> branch, I would do the following. Navigate to the local repository folder (using <code>cd</code>), then <code>git 
            checkout master</code>. This moves us into the master branch, then <code>git merge dev</code>, merges <i>dev</i> with <i>master</i>. You would then have to resolve 
            any merging conflicts that arise.</p>
            <p><b>GitKraken:</b> You should check into <i>master</i> then right-click on <i>dev</i> followed by <i>‘merge dev into master.’</i></p>
            <h1>Having more than one developer</h1>
            There are inevitable commits done by other developers in between your commits when there is more than one developer. After you have made your commit, but before you push it, you should pull the new commits. Remember, pull before you push!
            <p><b>Command: </b></p>In the case that you have multiple people working on one repository, you will need to account for their changes too. This requires the use of the <b>pull merge commit push</b> system, whereby just before you push your changes, you first pull from the directory using <code>git pull</code>, then git will merge in any changes performed by the other person. Note, it sometimes can’t do this, and you will have to manually select what code to keep, either yours, the other persons, or both. With the issues in the merge resolved, you then <code>git add</code>, <code> git commit</code> and <code> git push</code> as described previously.
            <p><b>GitKraken: </b>Use the pull button and <i>‘fast-forward if possible’</i> option.</p></div>
            
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
    name:"Page16",
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



