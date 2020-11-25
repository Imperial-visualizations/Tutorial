<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <div class="iv-main">
 <center>
            <h1>Slack</h1>
            </center>
            <p> Slack is the messaging service we use at Imperial Visulsations. Imperial Visualisations has two workspaces; one for code and crisps,  which you can find at
                <a href= "https://impviscodecrisps.slack.com">https://impviscodecrisps.slack.com</a>, and one for summer 
                students, which you can find at <a href="https://imperialvisualize.slack.com">https:/imperialvisualize.slack.com</a>.To join a workspace, you must receive 
                an invitation link to that workspace. Note to staff/summer team: Adding someone to a pre-existing workspace is
                simple, you just need their email, and follow the prompts following “invite people” beneath direct messages in
                the workspace you want to add them to. If you have not got an invitation link to the workspace yet, you need to
                request one by contacting Caroline Clewley at c.clewley@imperial.ac.uk. When you are added to a workspace, you
                will receive an email asking if you want to join that slack workspace, click join. This will take you to a tab 
                where you write your full name, enter your new slack password, then click create account.This should open slack 
                in the correct workspace, from here you can message people! Note, slack is quite useful as you can send code
                snippets in messages.
            </p>
            <p>
                When you want to log in again, just go to <a href ="https://slack.com/intl/en-gb/">https://slack.com/intl/en-gb/</a> and click
                 launch slack, your workspace will drop down, click on it and it’ll take you there.
            </p>
            <p>
                Slack is most effective if you download it to your computer and/or phone, and set the notifications to be alerted about new messages.
                Within a workspace, <i>channels</i> can be set up, where you can private message individuals or groups of people. Notifications can be set up 
                separately for each channel or private message. Once you have started developing a visualisation, we recommend creating a private channel
                for all the partners to discuss the visualisation development.
            </p>
            <p>
                 For Code & Crisps/STEMM students, the main open channels to monitor are:
                 <ul>
                    <li>#drop-in sessions: for news and info about Code & Crisps drop-in sessions;</li>
                    <li>=#learning_materials: for links to useful material in order to learn the relevant programming skills;</li>
                    <li>#visualisation_ideas: for posting new ideas for visualisations, plus the invitation link to edit the Trello board of visualisations in progress</li>
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
    name:"Page18",
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



