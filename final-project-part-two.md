| [home page](https://esha-pandya0203.github.io/esha-pandya-portfolio/) | [visualizing government debt](visualizing-government-debt) | [covid case map](covid-cases-map) | [critique by design](critique-by-design) | [final project I](final-project-part-one) | [final project II](final-project-part-two) | [final project III](final-project-part-three) |

# Wireframes / storyboards
For Part II, I developed the initial sketches from Part I into a more detailed storyboard using Shorthand. The draft follows a patient evaluating hospitals, beginning with an introduction to overall CMS hospital star ratings and progressing toward an examination of the individual quality measures that contribut to those ratings. The patient initially views a higher rating as a better performing hospital, but later learns that highly rated hospitals can have safety concerns. 

I also created preliminary data visualizations using Tableau and the [CMS Hospital General Information dataset](https://data.cms.gov/provider-data/dataset/xubh-q36u?conditions[0][property]=state&conditions[0][value]=PA&conditions[0][operator]=%3D), focusing on hospitals in Pennsylvania. I processed the data in Python to ensure Tableau had the correct rows and columns needed to create effective visualizations. These visualizations include the distribution of hospital star ratings, the five quality measure groups, comparisons between similarly rated hospitals, and an examination of selected safety measures. Altogether, the visualizations support the central message that a hospital's overall star rating provides a useful summary of quality but does not necessarily reflect performance on every measure. 

My storyboard is located on Shorthand [here](https://preview.shorthand.com/XLgl44OgzlPn9C8k). 

### Introduction: Hospital Star Ratings in Pennsylvanis 
Purpose: Establishes Context 
<div class='tableauPlaceholder' id='viz1795564577657' style='position: relative'><noscript><a href='#'><img alt='Dashboard 1 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Di&#47;DistributionofStarQualityRatingsinPennsylvania&#47;Dashboard1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='DistributionofStarQualityRatingsinPennsylvania&#47;Dashboard1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Di&#47;DistributionofStarQualityRatingsinPennsylvania&#47;Dashboard1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /></object></div>               
<script type='text/javascript'>                    
    var divElement = document.getElementById('viz1795564577657');                    
    var vizElement = divElement.getElementsByTagName('object')[0];                    
    if ( divElement.offsetWidth > 800 ) { vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';} 
    else if ( divElement.offsetWidth > 500 ) { vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';} 
    else { vizElement.style.width='100%';vizElement.style.height='727px';}                     
    var scriptElement = document.createElement('script');                    
    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    
    vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script>

### Understanding the Overall Rating 
Purpose: Explain the rating methodology 
<div class='tableauPlaceholder' id='viz1795564684935' style='position: relative'><noscript><a href='#'><img alt='Dashboard 1 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Br&#47;BreakdownofCMSStarQuality&#47;Dashboard1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='BreakdownofCMSStarQuality&#47;Dashboard1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Br&#47;BreakdownofCMSStarQuality&#47;Dashboard1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /></object></div>                
<script type='text/javascript'>                    
    var divElement = document.getElementById('viz1795564684935');                    
    var vizElement = divElement.getElementsByTagName('object')[0];                    
    if ( divElement.offsetWidth > 800 ) { vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';} 
    else if ( divElement.offsetWidth > 500 ) { vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';} 
    else { vizElement.style.width='100%';vizElement.style.height='727px';}                     
    var scriptElement = document.createElement('script');                    
    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    
    vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script>

### Same Stars, Different Results 
Purpose: Challenge initial assumption 
<div class='tableauPlaceholder' id='viz1795564714655' style='position: relative'><noscript><a href='#'><img alt='Dashboard 1 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Tw&#47;TwoHospitalsSameScoreDifferentFactors&#47;Dashboard1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='TwoHospitalsSameScoreDifferentFactors&#47;Dashboard1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Tw&#47;TwoHospitalsSameScoreDifferentFactors&#47;Dashboard1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /></object></div>                
<script type='text/javascript'>                    
    var divElement = document.getElementById('viz1795564714655');                    
    var vizElement = divElement.getElementsByTagName('object')[0];                    
    if ( divElement.offsetWidth > 800 ) { vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';} 
    else if ( divElement.offsetWidth > 500 ) { vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';} 
    else { vizElement.style.width='100%';vizElement.style.height='727px';}                     
    var scriptElement = document.createElement('script');                    
    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    
    vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script>

### Safety Analysis on Highly-Rated Hospitals 
Purpose: Main reveal, motive for questioning for the overall rating 
<div class='tableauPlaceholder' id='viz1795564748274' style='position: relative'><noscript><a href='#'><img alt='Dashboard 1 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;AH&#47;AHighlyRatedHospitalcanstillFailtoMeetSafetyBenchmarks&#47;Dashboard1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='AHighlyRatedHospitalcanstillFailtoMeetSafetyBenchmarks&#47;Dashboard1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;AH&#47;AHighlyRatedHospitalcanstillFailtoMeetSafetyBenchmarks&#47;Dashboard1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /></object></div>                
<script type='text/javascript'>                    
    var divElement = document.getElementById('viz1795564748274');                    
    var vizElement = divElement.getElementsByTagName('object')[0];                    
    if ( divElement.offsetWidth > 800 ) { vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';} 
    else if ( divElement.offsetWidth > 500 ) { vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';} 
    else { vizElement.style.width='100%';vizElement.style.height='727px';}                     
    var scriptElement = document.createElement('script');                    
    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    
    vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script>

### Exploring Individual Hospital Quality 
Purpose: Give patients a practical tool 
<div class='tableauPlaceholder' id='viz1795564777379' style='position: relative'><noscript><a href='#'><img alt='Dashboard 1 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;St&#47;StarRatingBreakdownExplorationforPAHospitals&#47;Dashboard1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='StarRatingBreakdownExplorationforPAHospitals&#47;Dashboard1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;St&#47;StarRatingBreakdownExplorationforPAHospitals&#47;Dashboard1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /></object></div>                
<script type='text/javascript'>                    
    var divElement = document.getElementById('viz1795564777379');                    
    var vizElement = divElement.getElementsByTagName('object')[0];                    
    if ( divElement.offsetWidth > 800 ) { vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';} 
    else if ( divElement.offsetWidth > 500 ) { vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';} 
    else { vizElement.style.width='100%';vizElement.style.height='777px';}                     
    var scriptElement = document.createElement('script');                    
    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    
    vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script>

Note that the lefthand side of the explorer is a work in progress in terms of removing excess labels. 

## Storyboard Walkthrough 

| Section | Intented Reader Understanding | Visualization |
| --------- | ---------- | ---------- |
| Introduction | What does a star rating mean? | Pennsylvania rating distribution |
| Understanding | What contributes to an overall rating? | Measure-group weighting chart |
| Comparing | Can similarly rated hospitals differ? | Hospital comparison |
| Main Reveal | Can highly rated hospitals have unfavorable individual measures? | Safety analysis |
| Conclusion | How should I use this information? | Three-step call to action & interactive explorer |

# User research 

## Target audience
The target audience for this project are patients and families who may need to compare hospital options before making healthcare decisions. The story is designed for individuals who do not necessarily have experience intepreting hospital quality metrics or working with healthcare data. Although the project focuses on Pennsylvania hospitals, the broader goal is to help patients understand how overall quality ratings can be understood and prioritize healthcare decisions based on personal preferences. 

For the user research, I plan to interview at least three adults with varying levels of familiarity with hospital ratings and healthcare decision-making. One paticipant will be comfortable navigating the U.S. hospital system, one participants will be new to the system, and the other will be somewhere in between to ensure that all levels of healthcare literacy can be supported through this project. 

## Interview script

| Goal | Questions to Ask |
|-------------|-------------------------|
| Understand familiarity with hospital ratings | Have you ever used hospital ratings or reviews when choosing a hospital? |
| Understand initial assumptions | If you saw a hospital with four out of five stars, what would that rating mean to you? |
| Check if readers understand distribution graph | Looking at this graph, what is the main takeaway you notice? What would you assume? |
| Assess understanding of breakdown | Is any part of the rating composition confusing? Does it require more clarity? | 
| Evaluate hospital comparisons | Does this visualization affect how you interpret the shared star rating? | 
| Check if readers understand safety analysis | Is the message of this visualization clear? Is anything about the benchmark or safety measures confusing? | 
| User preference for exploration feature | If you were choosing a hospital, what information would you like to see first? Is there anything in the explorer that is missing? | 
| Confirm overall message | What do you think is the main message of this story? | 

## Interview findings

| Questions  | Interview 1 (student, 20s, new to healthcare system) | Interview 2 (student, 20s, has some experience with healthcare system) | Interview 3 (physician, 50s, most experience with healthcare system) |
|-------------------------|--------------------------------|-------------|-------------|
| Have you ever used hospital ratings or reviews when choosing a hospital? | No | No, I have not (I stick with the same one as my parents and trust their opinion). | Yes |
| If you saw a hospital with four out of five stars, what would that rating mean to you? | I would think the workers are nice, the response time is fast, and the service is fast as well. | I would think that it is a pretty good hospital overall. | It depends on the number of total reviews. |
| Looking at this graph, what is the main takeaway you notice? What would you assume? | It makes me think that the most of the star ratings are 4 stars, then the second most rated is 3 stars, then the next category would be 2 stars, next 5 stars, and lastly 1 star with the lowest rating. | 4 stars are the most common rating in PA, followed by 3 stars, 5 and 2 are approximately the same amount, and very few hospitals have one star. | Most Pennsylvania hospitals do a better than average job. |
| Is any part of the rating composition confusing? Does it require more clarity? | What does CMS mean? What are the proportions of the pie chart (percentage/numbers)? | In the pie chart, at a quick glance it seems like mortality, patient experience, and safety of care are equally weighted. Maybe including the percentage weights would be useful alongside the list of weight priority. | It's clear and would prefer to have physician's ratings included. |
| Does this visualization affect how you interpret the shared star rating? | I am confused in the graph, 0 makes me believe that the star contribution is 0 stars? May if sorted from most stars to lowest? In that case, the pink would be first becuase it is the largest, and then put the actual count of how many stars each category has. | Yes! It quickly lets me see what hospitals perform better amongst the 5 groups and could help me decide which one to choose if I cared a lot about one of the 5 groups a lot. | Yes, it lets me decide which hospital I would visit based on safety of care and readmission rate instead of a generalized score. |
| Is the message of this visualization clear? Is anything about the benchmark or safety measures confusing? | I think it is. If I got it right, the graph is showing that red is the percentage of not safe and grey is safe. | To me, I think including both the percentage and number in the same bar is a little hard to read/confusing. And labeling the y-axis to show that is the star rating would be helpful as well to me! Overall, I can see that a small number of 4 star hospitals have 1 safety measure below CMS requirement, and even fewer for 5 star hospitals. | Elaborate what safety benchmarks are included in the rating. |
| If you were choosing a hospital, what information would you like to see first? Is there anything in the explorer that is missing? | How far is the hospital from my actual location? If friends have already visited any, I would ask for their feedback. | In addition to rating, I would want to see the histance from where I am to the hospital. If I don't particularly care about any of the 5 groups and was in between two four-star hospitals, I would pick the closest one. I also think in the explorer, it would be nice to compare 2 hospitals at once, like the visualization in the "Two hospitals: same score, different factors." | Be able to compare the hospitals. Put the legend closer to the donut chart. |
| What do you think is the main message of this story? | What makes a hospital safe? Are there any other measures that people can use to better choose which hospital to go to? | That hospitals with the same rating aren't the same and that it's useful to see what goes into these ratings depending on my needs. | Consumers need to be educated about making better decisions for their own care. |

# Identified changes for Part III

From conducting the interviews above, I realized I can make improvements on my existing draft to improve the readability and understanding of the audience. I've noted these changes below: 

| Research synthesis                       | Anticipated changes for Part III                                                |
|------------------------------------------|---------------------------------------------------------------------------------|
| The proportions in the rating breakdown pie chart are unclear and readers are guessing. | Add percentages to the pie chart itself. |
| It is unclear what measures go into the safety analysis. | Include the specific metrics that go into the safety measure group. Add more clear axis labels for the visualization. |
| The explorer lacks some information that a user would normally use to make an informed decision. | Allow the user to directly compare two hospitals side-by-side. Also add a map so user's can see their location relative to the hospitals in the area. |                                                                       |

Overall, the interviewees understood the overall message of the story, requiring more clear labels in the visualizations to better and more efficiently understand the point. 

For Part III, I plan to develop the final storytelling experience as a React web application. This will allow me to customize the visual design and organize the Tableau visualizations into a more cohesive narrative. The website will retain the central structure developed in Part II, moving from an introduction to hospital star ratings toward a deeper examination of individual quality measures and an interactive hospital explorer. The overall story and visualizations will remain consistent with the current drafts, with the refinements mentioned above. 

## References
- Hospital General Information | Provider Data Catalog. (n.d.). Retrieved November 16, 2026, from https://data.cms.gov/provider-data/dataset/xubh-q36u#data-table

## AI acknowledgements
I did not use AI to complete Part II of the final project. 