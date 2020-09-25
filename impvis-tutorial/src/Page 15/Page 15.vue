<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <div class="iv-main">
<center>
            <h1>Making and pushing a commit</h1>
            </center>
            <p> Once you have done some changes to your code and are happy with your progress, you may want to save (push) 
            it to the repository on Git. The first step is to make a commit of the changes you like.Having a commit in the GitHub history when stuff is working is great because if you accidentally make some mistakes in your 
                code and can't change them, then reverting to these commits (savepoints) is precisely what you need. Always keep this in mind! 
                Make sure to commit your code with a descriptive message as frequently as possible even if it's not working; that way, you can 
                always go back to something that was slightly less broken if the situation worsens. Avoid pushing straight to master; instead,
                 push your changes to a separate branch and then merge into master.</p>
            <p><b>Command:</b> Git commands are performed inside of the cloned git repository. First, you must navigate to the folder 
            inside of the command line. Once there, run <code>git status</code> to see how many commits, and you are ahead of or behind origin. To 
            commit something, we first have to identify the files we want to add to the commit; this can be done by adding individual 
            files using <code>git add <i>myFileName</i></code> or to just add all the files in the repository just use <code>git add</code>. This is the lazy option but
             very effective. Once all the desired files are added, you then commit them; this is done via <code>git commit -m <i>``message describing 
             the commit, what have I changed or done”</i></code> the message associated with the commit is vital, as it lets you know what you were
              doing at this point, should you need to revert future code to this point. Now that you have committed, you want to push 
              those changes to the remote directory so that other people can access them. This is done using <code>git push</code>. 
            </p>
            <p><b>Gitkraken:</b>GitKraken will tell you the file changes in the working directory. You should click on <i>‘view the changes.’</i>
            In the <i>‘Unstaged Files’</i> section, you should be able to click on the files that have changes to them and view the changes comparing 
            line by line before and after the change. At this point, you still can decide whether to keep certain changes by using the <i>‘Discard
            Hunk’</i> (remove this change) and <i>‘Stage Hunk’</i> (put this change into the drafted commit) buttons. If you are sure of all, you can use 
            the <i>‘Stage all Changes’</i> button without checking every single changed file. Similarly, you can try to revert all the changes using 
            the <i>‘Discard All Changes’</i> bin button. Once you have checked all the changes, you should write the commit message and press the commit
            button. If no new changes are coming from the Git, you should be able to push the commit to Git. If the push is successful, you have
            now made the changes on Git!
            </p>
            </div>
            
        </iv-visualisation>
    </div>
</template>
<script>
export default {
    name:"Page15",
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



