<template>
    <div>
        <iv-title-bar>ImpVis tutorial</iv-title-bar>
        <iv-visualisation>
            <center>
            <h1>Visualisation development cycle</h1>
            <h2>4 a1. Identifying the primary learning outcome</h2>
            </center>
            <p>When creating or improving a visualisation, the most important thing is to clarify what the 
            visualisation is trying to achieve. Please spend some time thinking about the key realisations 
            you want your user to have, and how to place them in a well-ordered manner. The learning process 
            should be as transparent as possible. Think about what the user already knows; what knowledge do 
            you assume? Do they need refreshing on some of the key concepts that'll be used later?</p>
            <p>The title of a visualisation is essential. Be clear on actually what the content of a visualisation is. 
            So, for example, instead of having "Fourier series" as a title, something like "Deconstruction and reconstruction 
            of functions through Fourier series" would be much better.</p>
            <center>
                <h2>4 a2. Secondary learning outcomes and learning steps (for suites/advanced writers)</h2>
            </center>
            <p>
                When creating a visualisation, it’s important to think of the key learning steps you want the user to have. 
                Think about how many steps you want to make. Currently, visualisations have between 4 and 6 pages, typically 
                with one ‘learning step’ per page. You may feel this is about right for the content you will be demonstrating, 
                but this may be either too many or too few. Perhaps you only need 2 or 3 pages to explain the topic thoroughly 
                or for complicated topics that build up through a lot; 9 or 10 pages might be a better idea.
            </p>
            
            <p>
                An excellent way to list these steps and to decide how many to have is to write down subtitles that you think 
                each page deserves, where this sub-title describes what that page’s learning step will be in just two or three 
                words. This makes it more evident to the user the main result they need to take from that page and makes the 
                visualisation more comfortable to navigate if they need to return to anything. It also helps you keep track of 
                the structure of the learning journey when creating a visualisation.
            </p>

            <p>
                When creating a visualisation, it's important to consider the style of page Imperial Visualisations uses. The 
                left third of the page is currently a scrollable page that will explain the content, so any theory or derivations 
                would go here. The middle and right third of the page will then be dedicated to the interactive part of the visualisation. 
                Anything that can be clicked, dragged, or played with goes there. If this isn't clear, check out the Fourier series 
                visualisation, this is a working model for the style we're going for.
            </p>
            
            <p>
                Note, you don't want the user to have to scroll on the page's right-hand side. The idea is that the user scrolls 
                on the left-hand side of the page, reading the content/explanations. When they've reached a section where the next 
                visualisation is more relevant, the right-hand side updates and shows new interactive material which they'll go on and 
                use. Appropriately done, this gives the learning journey a good structure, as interactive material is revealed to them as they build up their knowledge of the topic at hand.
            </p>

            <p>
                <i>Khan Academy</i> and <i>Coursera</i> are great places to look for well thought out learning journeys; check these out! 
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



</style>



