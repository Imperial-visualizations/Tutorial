<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <template #hotspots>
                <iv-pane position="left" :width ="550">
                    <img src="@/assets/images/core_team.png"  style="width:400px;height:auto;"/>
                    <br>The underlying structure to a visualisation development team.
                </iv-pane>
            </template>
            <div class="main-content">
                <h1>Who are we, and what do we do?</h1>
                <!--<h2>For code and crisps students:</h2>-->
                Imperial Visualisations is a team of staff and students from across College. We create interactive online visualisations on abstract concepts in conjunction with lecture courses.  The core team is composed of four groups of people. These are:
                <ul>
                    <li><b>Staff partners</b>: College staff members with expertise in an academic subject.</li>
                    <li><b>Research partners</b>: Collaborators investigating the educational impact of our project and usage of the visualisation (can be both staff and students).</li>
                    <li><b>Student partners</b>: Students, experts in learning, with recent insight into the pros and cons of the modern teaching of their subject.</li>
                    <li><b>Summer team</b>: A group of students of engage with the project over the summer with the aim of innovation & development.</li>
                </ul>
            </div>
        </iv-visualisation>
    </div>
</template>
<script>

export default {
    name:"Page-2",

}
</script>
<style>
.main-content{
    text-align:center;
}

ul {
    list-style-type: none;
}
</style>



