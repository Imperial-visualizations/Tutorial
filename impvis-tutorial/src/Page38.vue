<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <center>
            <h1>4c1 - Designing a visualisation</h1>
            </center>
            <p>
            The structure of individual visualisations is such that explanatory text is 
            positioned to the side of main visualisations that may be <i>overlaid</i> onto the main 
            interactive part of the visualisation itself or push the visualisation into a more 
            narrow window. A "vis" component lies at the back of the whole visualisation. 
            This houses all components built up on top of one another, other than the title bar 
            and the guidance system. 
            </p>
            <p>
                In order of increasing height, we have “vis,” which houses everything. On top of 
                this, “Pane” and “mainstage” are used. Panes are designed to accommodate the 
                bulk of text content, while the mainstage houses interactive content. Multiple 
                panes can be used on any side of the mainstage. Still, most of our visualisations 
                so far have chosen to have a single pane to the left of the mainstage. The panes are 
                at the same height as the mainstage.
            </p>
            <p>
                Inside the Pane can go any of the other components, emphasizing usage for text; 
                for example, text dropdowns. The Pane is toggleable and draggable, in that it can 
                be dragged wider/thinner to show more/fewer words per line, and that there is a click 
                to open/close button which moves it on/off the screen.
            </p>

            <p>
                The mainstage can also house any of the other components (apart from Panes), focusing on 
                interaction. In particular, these house the hotspots - used to keep the layering system well
                organised and clean. They act as anchors within the mainstage on which components appear on top 
                of the mainstage land.
            </p>
            <p>
                There are currently two different types of hotspots, togglable, and fixed. Fixed hotspots 
                can be used to contain elements that need to be seen at all times but are distinct from the 
                main stage visualisation. Toggable hotspots act as a small dockable component; they are meant 
                to contain essential components to the visualisation but don't need to be seen at all times. 
                This might include buttons, sliders, checkboxes, and small graphs, etc. There are four corner 
                hotspots and then four edge hotspots that lie in between. These edge hotspot areas can contain
                multiple sub hotspots, unlike the corners. Within a single hotspot, you can stack several block 
                elements such as a sliderBlock, which have been pre-made to be easy to set up - think IKEA. Note, 
                if you have panes either side of the visualisation, (e.g., a pane on the left-hand side), then it's 
                advisable not to use components in hotspots on the same side as panes (i.e., on the left-hand side in this case). 
                This is because the Pane may cover the component in the hotspot if dragged.
            </p>

            <p>
                The guidance system intends to aid the visualization user in understanding how to get as much as 
                possible out of the experience. It is not to be used to explain scientific concepts. However, the 
                visualization components may be used in such a manner if they aren't used within the guidance system, 
                e.g., the window modal component. For more on the guidance system, see section 4b.
            </p>
            <p>
                The visualisation page's complexity should decrease the further the user gets from the main visualisation 
                stage/canvas. Practically speaking, this meant that you shouldn't have text in the main stage of the 
                visualisation. Alternatively, it would be best if you didn't have complex graphs or models within a side pane 
                or togglable hotspot. Suppose you find yourself requiring a more complex visualization as an add on to highlight 
                some scientific concept that is adjunct to what you are explaining in the main stage visualization. In that case, 
                you likely need to make another visualisation page entirely. So, for example, if I have an interactive quiver plot 
                visualisation showing the electromagnetic field around a bar magnet within the mainstage, you might also want to 
                include a graph of the integral of the magnetic field around a path. This second plot would be an ideal candidate 
                to put into a side pane or hotspot. It adds to the user's understanding of EM but is distinctly less complicated 
                that the main vis.<redText>(Perhaps a less jargon heavy example could be used here, either that or we could make an 
                    actual exampe showing what is meant)</redText>
            </p>

            <p>
                A note on default values and initial reaction to a visualization: The concepts being displayed should be evident 
                for the user to at least anticipate before reading the text. The changes that occur due to moving different sliders/buttons 
                should easily be noticed right from the start. The key to this is picking sensible 'default' settings that the user sees upon 
                reaching this suite's visualization. A good way to determine if default settings are chosen sensibly is if the part of a 
                visualisation that changes under some slider/parameter change is visually sensitive to changes near the default values, but 
                not in an extreme limit of the behaviour seen in that part of the visualisation. This way, a user doesn't necessarily have to 
                interact with the visualisation before they somewhat understand what is going on. For example, if you check out the Fourier series 
                suite, one of the key points is how the number of terms changes an approximation to a function. Choosing an intermediate value of 3, 
                which shows some wiggles, but not too many, is much better than choosing 0, where the user can't see much yet and has to interact 
                to at least guess what's going on. Another example would be  100, where the approximation is almost perfect; the user might get 
                confused upon seeing it.
            </p>
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
redText 
{ 
    color: red; 
} 


</style>



