<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <div class="iv-main">
            <h1>Step 2: Opening the service and signing in</h1>
            <p><b>Command:</b> You may search in your machine for Command Prompt or Terminal.</p>
            <p><b>GitKraken:</b> Open a GitKraken window from wherever you saved it. Opening GitKraken can sometimes take a few minutes. Once you see picture 1 (see left pane)
            Click “Sign in with GitHub.” That should take you to a screen which looks like picture 2.</p>
            Click “Continue authorization.” That should take you to a GitHub login page (picture 3).
            Use your already made GitHub username and password. If you authorized your email for your GitHub account earlier, then signing in correctly there will take you to the page as seen in picture 4.
            Click “Authorize Axosoft.” Once you have done this, you will see <center><img src="@/assets/images/Success.png"  style="width:250px;height:250px;"/></center>
            This means you can safely close that tab and go back to your Gitkraken window. Opening this will take you now to “Set up your profile,”
             where you choose your avatar and account name. Go ahead and agree with the terms and conditions. No need to start a free trial of GitKraken
            pro, their free version does everything we need.
            </div>        
            <template #hotspots>
                <iv-pane position="left" width ="550">
                    <div class="sidebar-img">
                   Picture 1:
                    <center><img src="@/assets/images/Authorizing_Gitkraken.png"  style="width:150px;height:auto;"/></center>
                    Picture 2:
                    <center><img src="@/assets/images/gitkraken_login.png"  style="width:200px;height:auto;"/></center>
                    Picture 3:
                    <center><img src="@/assets/images/sign_in_to_continue.png"  style="width:200px;height:auto;"/></center>
                    Picture 4:
                    <center><img src="@/assets/images/Authorize_axosoft.png"  style="width:200px;height:auto;"/></center>
                    </div>
 
                </iv-pane>
            </template>

        </iv-visualisation>
    </div>
</template>
<script>
export default {
    name:"Page10",
}
</script>
<style>
.iv-main{
    margin:10px 50px;
}
.sidebar-img{
    height:100%;
    overflow-y:auto;
}
</style>



