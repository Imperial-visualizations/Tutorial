<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <div class="iv-main">
 <center>
            <h1>While coding: 4b. ImpVis Components and Vue</h1>
            <h2>Guidance System review</h2>
            </center>
            <p>
                So how does it work? Or at least how is it intended to work? The user interacts in two different ways, 
                firstly accessing the information on individual items using buttons stored within the iv-visualization 
                component. This includes most of the screen, excluding the title bar. When clicked, a modal appears showing 
                help on specifically only that component. The second is a more general system used for a user who quickly 
                wants to understand how to use all the visualization items. This allows the user to pick a branch to go 
                down intended to show several screens of information regarding a common theme, such as graphs or sliders. 
                There is also the option to see all the modal screens in one go.
            </p>
            <center><h2>Z-indexing</h2></center>
            <p>When a modal is shown, an HTML element may be highlighted by showing it above the greyed out modal background. 
                This is currently achieved by changing the z-index of the selected HTML element and then returning to z-index=0 
                after the window is close, or a new screen is selected. Z-index is tricky in that the parent of the component 
                determines the ceiling of the child component regardless of that child's z-index. The top element's z index determines 
                the z index of its children. However, the z-index of any of the children can be set. See here:#
            </p>
            <p><center>
                Examples:
                <ul>
                    <li>Parent 1 : 0
                        <ul>
                            <li>Child a : 0
                                <ul>
                                    <li>Child: b : 900</li>
                                </ul>
                            </li>
                        </ul>
                    </li>
                    <li>Parent 2 : 0
                        <ul>
                            Child q: 500
                        </ul>
                    </li>
                </ul>
            </center>
            </p>
            <p>
                Even though child b is from a parent at the original source with the same z-index as the sibling 
                because it has a child with a set z-index above it, then the z-index of child a is compared to child q. 
                Hence, child b is never above child q. In the image above, the z-index is used to highlight a specific 
                component associated with the guidance help screen, which is the top left togglable hotspot. This is 
                achieved by having the guidance system z-index set to 0 and the iv-visualisation component z-index set 
                to 0. None of the children of these two components has a z-index set, which itself has children. This 
                means that its okay to have an individual button, which is a child of iv-visualisation with a z-index set 
                to say 1. Still, the button itself should not have children with a set z-index. As outlined earlier, these 
                children will always have their z-index relative to the parent button and not to some absolute z-index. 
                In the image's case, the guidanceModal component raises the highlighted component to be at a z-index higher 
                than the grey background but underneath the actual modal. When the modal screen is closed or changed, the 
                highlighted component is returned to the <b>z-index: auto</b> state:
                <center><img src="@/assets/images/z_index_display.png"  style="width:549px;height:266x;" align = "down"/></center>
            </p>
            <h2>Guidance System review</h2>
            <p>The guidance data structure is constructed currently as shown below.</p>
            <center><img src="@/assets/images/guidance_data_structure.png"  style="width:1009px;height:372x;" align = "down"/></center>
            <p>
            Each individual modal help screen requires the following: text, highlightDiv, identifier, position, and colour_rgb. 
            Text is what is shown inside of the modal body.  HighlightDiv is the HTML element, which is highlighted by the guidance 
            (this should be sensible, i.e., don't highlight something within another hotspot if your guidance button is in another hotspot). 
            The identifier is used to link the guidanceButton within a component to a specific item within the guidance file system, 
            positonModal is used to position the modal on the screen <span class="red">[need clarification (from Dan..) on how this works]</span >.
            Finally, clour_rgb sets the main theming colour of the modal, which is used to calculate several shades and tints used in the modal 
            design, i.e. [r_value,g_value,b_value]. The same model unit may be put in different branches as long as it is precisely the same 
            i.e., doesn't have a different text for the same identifier. The current system will, however, be changed to one using markdown files 
            for more flexibility. 
            </p>
            <p>
                Associated with this data structure in App.vue, the main components in the HTML of the vue file may look like this:
                <center><img src="@/assets/images/component_organisation.png"  style="width:1131px;height:470x;" align = "down"/></center>
            </p>
            <p>
                Please see the wiki of individual components for more specifics. Still, the overall notes are that the <b>iv-guidance-system</b>
                component must be included above the <b>iv-visualization</b> component for the guidance system to work. That guidance buttons 
                with a valid identifier must be included to access a specific guidance modal.
                <center><img src="@/assets/images/component_organisation_display.png"  style="width:512px;height:250x;" align = "down"/></center>
            </p>
            <p><span class="red">Need a section of using the button</span >
            </p>
            </div>
           
        </iv-visualisation>
    </div>
</template>
<script>
export default {
    name:"Page46",
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
.red 
{ 
    color: red; 
} 

</style>



