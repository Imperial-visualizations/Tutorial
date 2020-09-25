<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <center>
            <h1>Trello</h1>
            </center>
            <p>We use Trello to keep track of everything.  Signup to Trello at <a href="https://trello.com/en-GB">https://trello.com/en-GB</a>. Once 
            you’ve made an account, you have to verify your email address, don’t forget to do this! It only takes 1 minute. Once your account is set up,
            Trello asks you to make a team. If you don’t need to do this, just make a dummy team with a random name and purpose, and don’t bother adding
            anyone to this team.
            </p>
            <p>
                Once you have set up an account,you need to be added to a team to visit it.
            </p>
            <p>
                Note to staff: To add a new team member, under <i>“Imperial_Visualizations”</i> in <a href="https://trello.com/impvis/home">https://trello.com/impvis/home</a>, there is a “members” button. Click this button, then click <i>“Invite team members”</i> to invite someone to the team. Type their email and click <i>``add to team''</i>'.
            </p>
            <p>
                Once you’ve been added to a team, you should be able to check out our board at <a href ="https://trello.com/impvis/home">https://trello.com/impvis/home</a>. From here you’re all set.
            </p>
            <p>
                In particular, you will be interested in <a href="https://trello.com/b/mR6L3TtH/visualisations-in-progress">https://trello.com/b/mR6L3TtH/visualisations-in-progress</a>, which is where we
                 keep track of all of our visualisations in progress. Note, anyone can view this, but to edit it, you need to be invited
                  and will be sent a link on <i>Slack</i>. A list represents each visualisation with its status, staff partner, student partner, 
                  department/course, and description. The best method to create a new visualisation list is to copy an existing list and 
                  edit the details. The status needs to be updated as the visualisation progress and is colour coded:
                <ul>
                    <li><span class="green">Green:</span> Looking for student partner(s).</li>
                    <li><span class="yellow">Yellow:</span > Looking for staff partner(s).</li>
                    <li><span class="purple">Purple:</span> In development.</li>
                    <li><span class="dark-blue">Dark Blue:</span> Under review.</li>
                    <li><span class="light-blue">Light Blue:</span> Being improved (further development after review).</li>
                    <li><span class="navy">Navy:</span> Live (uploaded to website).</li>
                </ul>
                When you click on the status, you will also see a checklist for each phase of the development process: these get ticked off upon completion of the relevant sections.
            </p>
            

        </iv-visualisation>
    </div>
</template>
<script>
export default {
    name:"Page19",

}
</script>
<style>
div {
  padding-top: 10px;
  padding-bottom: 50px;
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

span{
    font-weight: 600;
}
.red
{ 
    color: red; 
} 
.green 
{ 
    color: green; 
} 
.yellow
{ 
    color: yellow; 
} 
.purple
{ 
    color: purple; 
} 
.dark-blue
{ 
    color: darkblue; 
} 
.light-blue
{ 
    color: lightblue; 
} 
.navy 
{ 
    color: navy; 
} 


</style>



