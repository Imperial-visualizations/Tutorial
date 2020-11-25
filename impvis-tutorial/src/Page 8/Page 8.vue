<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <div class="iv-main-content">
            <center>
            <h1>Get connected</h1>
            </center>
                Before you get started and connected, you may want to see some of our current visualisations on <a href="www.imperialvisualisations.com">our website</a>!
                GitHub is used to store all of the code used to create the visualisations. Once the developer (you) has set up a repository on 
                GitHub, either command or GitKraken are used to make a copy of the repository on GitHub and store it locally (on your computer).
                From here, you can edit it. Communication between collaborators of a particular visualisation is  Slack is used to communicate with all the collaborators of a particular visualisation. We use Trello to keep track of all the tasks that need completing to move forward with a visualisation. Documented below is how to use all of these tools and services: 
                Summer team:
            <h2>Github: </h2><p>We store and share our visualisations code on Github.</p>
            <p>If you don’t have a GitHub account, follow the instructions 
            <a href="https://github.com/join?ref_cta=Sign+up&ref_loc=header+logged+out&ref_page=%2F&source=header-home">here</a>.
            You will need a new username and an email address; your college email should be fine! Once you have 
            completed your setup (don’t worry too much about customization along the way), you will receive a 
            verification email on your registered email account. Open the email and click “verify email address.” 
            Doing this will open GitHub logged into your new account and ask what you want to do first. If you 
            wish to learn more about GitHub, you can follow one of their suggested options. However, you can skip 
            if you only want to use GitHub for imperial visualisations for now.</p>
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
    name:"Page8",
}
</script>
<style>
.iv-main-content{
    margin:10px 50px;
}
</style>



