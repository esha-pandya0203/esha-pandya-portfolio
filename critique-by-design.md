| [home page](https://esha-pandya0203.github.io/esha-pandya-portfolio/) | [visualizing government debt](visualizing-government-debt) | [covid case map](covid-cases-map) | [critique by design](critique-by-design) | [final project I](final-project-part-one) | [final project II](final-project-part-two) | [final project III](final-project-part-three) |

# Visualization Redesign: Substance Use and Education 
For this assignment, I explored how reported substance use varies across educational backgrounds using the Drug Consumption (UCI) dataset. I followed a five-step design process: selecting an existing visualization, evaluating its effectiveness, sketching alternatives, collecting user feedback, and building an improved visualization in Tableau.

My final visualization allows users to select a substance and compare the percentage of respondents within each education group who reported using that substance at least once. 

## Step one: the visualization
**Original visualization:** [Drug Consumption (UCI) — Tableau Public](https://public.tableau.com/app/profile/r.nithyanandam/viz/MakeoverMonday2025Week41DataConsumptionsUCI/Dashboard1)

**Makeover Monday:** [2025, Week 41](https://makeovermonday.vercel.app/submissions/2025/41)

**Dataset:** [Drug Consumptions (UCI) — Kaggle](https://www.kaggle.com/datasets/obeykhadija/drug-consumptions-uci?resource=download)

As a healthcare analytics student, I selected the Drug Consumption (UCI) visualization because I was interested in how substance-use patterns differ across educational groups. The original Tableau dashboard (shown below) shows a heatmap of substance-use recency across several substances, ranging from alcohol and caffeine to cannabis and other drugs. An important note is that Semeron is a fictitious drug used to verify whether an individual is telling the truth. 

The visualization includes both respondent counts and percentages, and allows users to filter by age and gender to understand trends in different demographic groups. However, the information is densely organized, which makes it difficult to identify meaningful comparisons quickly. I saw an opportunity to simplify the information and explore a more specific analytical question using the same dataset. 

<div class='tableauPlaceholder' id='viz1794453729132' style='position: relative'><noscript><a href='#'><img alt='Dashboard 1 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Ma&#47;MakeoverMonday2025Week41DataConsumptionsUCI&#47;Dashboard1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='MakeoverMonday2025Week41DataConsumptionsUCI&#47;Dashboard1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Ma&#47;MakeoverMonday2025Week41DataConsumptionsUCI&#47;Dashboard1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /></object></div>                

<script type='text/javascript'>                    
    var divElement = document.getElementById('viz1794453729132');                    
    var vizElement = divElement.getElementsByTagName('object')[0];                    
    if ( divElement.offsetWidth > 800 ) { vizElement.style.width='1366px';vizElement.style.height='795px';} 
    else if ( divElement.offsetWidth > 500 ) { vizElement.style.width='1366px';vizElement.style.height='795px';} 
    else { vizElement.style.width='100%';vizElement.style.height='727px';}                     
    var scriptElement = document.createElement('script');                    
    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    
    vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script>

## Step two: the critique
I evaluated the original visualization using Stephen Few's *Data Visualization Effectiveness Profile*. The framework considers seven dimensions: usefulness, completeness, perceptibility, truthfulness, intuitiveness, aesthetics, and engagement. 

**What Worked:**

- **Color**: The red callouts stood out to me on an initial glance, highlighting the highest percentage/reported use categories. 
- **Detail**: The visualization itself contains detailed information with each cell representing the number of respondents and corresponding percentage. This allows the reader to see precise values aside from relying on color. 
- **Interactivity**: The age and gender dropdown filters work well to facilitate exploration of the differences between demographic groups. 
- **Consistent Organization**: the visualization has strong organization since all usage categories are applied to each substance, creating a grid-like structure. Categories where no data exists are represented by a white square. 

**Opportunities for Improvement:** 

- **Meaning of Color**: Although the red is a highlight color, a legend would help the reader interpret the color as a high percentage rather than increased risk of substance use. 
- **Visual Density**: The wide variety of substances (19) can clutter the heatmap, making it difficult for the reader to compare statistics across two drugs on opposite ends of the heatmap without increasing eye travel. The reader may be overwhelmed by the level of detail contained in one visualization. 
- **Missing Takeaway**: The title itself is also descriptive but not insightful, so the reader does not know what trends to look for. This appears to be more of an exploratory graph. 
- **Readability**: The abbreviated drug labels make the visualization less accessible to unfamiliar readers.

A breakdown of my evaluation results using Stephen Few's framework are as follow (note that each category was rated on a scale of 1-10): 

- Usefulness (7): The chart provides useful information for comparisons but no clear trend or insight label to guide readers. 
- Completeness (6): It includes detailed percentages and counts, but it also lacks visible explanatory context and a legend. 
- Perceptibility (3): The dense grid, small text, and abbreviated labels make patterns difficult to compare. 
- Truthfulness (8): The visualization uses an identifiable data source, but the color scale is unexplained and survey limitations are not described. 
- Intuitiveness (5): The heatmap structure and filters are familiar to most readers, but the lack of textual context can confuse the message sent to the readers. 
- Aesthetics (5): The graph has an organized grid and consistent font choices, but the gradient used in the heatmap is not balanced well. The dark grey overwhelms the visual palette. 
- Engagement (8): Interactive filters help with data exploration, but the lack of a takeaway limits how much users will engage with the visualization since they are unsure of what the message is. 

The primary audience is most likely researchers or students reviewing public health data to explore substance-use patterns. The visualization is effective for reaching the audience because it provides all the statistics that researchers and students would be looking for as well as allowing filtering based on demographic features like age and gender. The cluttered view of the heatmap deters most users from sitting with the chart to try and analyze it, making it geared towards someone invested in the subject. 

In my redesign, I want to focus on reducing the amount of data and instead show a pattern or trend directly through a different kind of visualization. I appreciate the filters for user customization in the original graph, so I want to repurpose those in another way, such as filtering by drug. Semeron is a fictitious drug used to keep survey results honest, and I think it would be useful to include in the caption and potentially highlight it so readers know it is different from the others. 

From the Good Charts reading, the process will include some data-driven exploration visualizations, iterating over multiple charts to determine which statistics I want to use to inform the readers. In general, the Good Charts method focuses on the relationship between the intended audience and the information being communicated in an easy-to-perceive format. Stephen Few's methodology identifies design weaknesses through separate criteria, distinguishing the benefits of certain features and drawbacks at the same time. A limitation of the scale created by Stephen Few is that assigned scores depend on the evaluator's judgement leading two people to agree or disagree about a specific category. 

## Step three: Sketch a solution
After critiquing the original visualization, I developed two sketches that explored different approaches to communicating information from the dataset.

<img src="substance-use-sketches.jpg" width="700"/>

**Sketch 1: Education Level and Substance Use**

My first sketch focused on comparing reported substance use across education levels. I used a vertical bar chart with education categories along the x-axis and counts along the y-axis. I also included a dropdown to let users select a specific substance. Unlike the original heatmap, this design uses education level as the primary comparison. I wanted to investigate whether substance-use patterns differed across educational backgrounds. The education level with the highest usage would be highlighted. 

**Sketch 2: Most Commonly Used Substances**

My second sketch focused on comparing the substances most commonly reported as used within the past month. Because the categories of usage recency are mutually exclusive, this graph would require grouping together counts of substance use reports. I used a horizontal bar chart to make comparisons across substances easier. This concept was more directly related to the original heatmap because it retained substance-use frequency as the primary focus. The most commonly used substances would be highlighted in a different color. 

**Selecting a Direction**

I preferred the first sketch because it explored a different question that interested me: how reported substance use varies by education level. Although this approach differed from the original visualization's main focus, it   uses the same underlying dataset and improves the clarity of the comparisons.

## Step four: Test the solution
The interviewees were shown both sketches, but the discussion focused on Sketch 1 (education-focus). 

Questions asked to Interviewees: 
1. What resonates with you the most from the visualization? 
2. Can you describe to me what this is telling you?
3. Is there anything you find surprising or confusing?
4. Is there anything you would change or do differently?

Results: 
- Interviewee 1: MSISPM Student, Second-year 
- Interviewee 2: MISM Student, Second-year 

| Question | Interview 1 | Interview 2 |
|----------|-------------|-------------|
| 1 | Emotional connected to the topic as college students | More storytelling |
| 2 | The visualization is trying to show which education-level has more substance use | How many people in each education level use different substances |
| 3 | The counts on the y-axis are not intuitive, the certification education level is not something that I would normally think of | Would replace the counts with percentages |
| 4 | Try a descending order of bars | Add an explanation as a caption of the patterns shown |

Synthesis: 
From the feedback I received, I got confirmation to proceed with Sketch 1 as my final visualization focus. We discussed the layout of the graph, the units used on the axis, and the order of the bars. During the interview process, I clarified that the title was subject to change depending on the visualization of the actual dataset. Although I initially thought to use counts (number of respondents) as the unit for the y-axis, I learned that this was not intuitive and to use percentages instead. This way, the graph would capture each education level's predisposed likelihood of substance use rather than overall comparison since the data is not reflective of the population. I also had to finalize how to display the percentage as either: (1) a percentage of all respondents or (2) a percentage of respondents within an education level. I ended up choosing the latter as it helped show my message more clearly and accurately. Design-wise, I knew I wanted to experiment with the layout to make it more readable as the "Certification" education level was unclear. 

## Step five: build the solution
<div class='tableauPlaceholder' id='viz1794452563740' style='position: relative'><noscript><a href='#'><img alt='Dashboard 1 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Ho&#47;HowDoesReportedSubstanceUseVarybyEducationLevel&#47;Dashboard1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='HowDoesReportedSubstanceUseVarybyEducationLevel&#47;Dashboard1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Ho&#47;HowDoesReportedSubstanceUseVarybyEducationLevel&#47;Dashboard1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /><param name='filter' value='publish=yes' /></object></div>                

<script type='text/javascript'>                    
    var divElement = document.getElementById('viz1794452563740');                    
    var vizElement = divElement.getElementsByTagName('object')[0];                    
    if ( divElement.offsetWidth > 800 ) { vizElement.style.width='1000px';vizElement.style.height='527px';} 
    else if ( divElement.offsetWidth > 500 ) { vizElement.style.width='1000px';vizElement.style.height='527px';} 
    else { vizElement.style.width='100%';vizElement.style.height='727px';}                     
    var scriptElement = document.createElement('script');                    
    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    
    vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script> 

The final dashboard displays the percentage of respondents within each education group who reported having used the selected substance at least once in their lifetime. Users can select a substance from the dropdown to update the chart. For each education level, the percentage is calculated as:
`Usage percentage = (Respondents in that education group who reported using the selected substance / Total respondents in that education group) × 100`

A respondent is considered to have reported lifetime use if their usage-recency response falls into one of the following categories:
- Used over a decade ago
- Used in the last decade
- Used in the last year
- Used in the last month
- Used in the last week
- Used in the last day

"Never Used" responses are excluded from the numerator. When all substances are selected, a respondent is counted as having reported use if they used at least one included substance.

### Final Design Decisions
| Design Decision | Reasoning |
|---|---|
| Horizontal bar chart | Makes category labels and bar lengths easier to compare |
| Education categories | Focuses the analysis on differences across educational backgrounds |
| Percentage instead of count | Accounts for differences in the sizes of education groups (change made based on interview) |
| Interactive substance filter | Lets users explore different substances without displaying numerous charts |
| Consistent education ordering | Maintains a logical progression between education categories |
| Gradient color palette | Organizes the education levels from least (lighter shade) to most (darker shade) usage |
| Explanatory caption | Clarifies how the percentages are calculated and interpreted to avoid reader confusion |

### What the Redesign Shows
The redesign provides a way to compare reported lifetime substance-use prevalence across education categories for a selected substance. The interactive filter makes it possible to investigate how these patterns vary depending on the substance. Unlike the original heatmap, which displays many substance-use categories simultaneously, the redesigned chart focuses on one comparison at a time. These results describe the survey sample and should not be interpreted as representative of the general population. Additionally, the analysis is observational and does not establish that education causes differences in substance use as use differs depending on the substance. 

## References
1. R. Nithyanandam. [Drug Consumption (UCI), Tableau Public](https://public.tableau.com/app/profile/r.nithyanandam/viz/MakeoverMonday2025Week41DataConsumptionsUCI/Dashboard1).
2. Makeover Monday. [2025 Week 41 Submissions](https://makeovermonday.vercel.app/submissions/2025/41).
3. UCI Machine Learning Repository. [Drug Consumption (Quantified)](https://archive.ics.uci.edu/dataset/373/drug-consumption-quantified).
4. Kaggle. [Drug Consumptions (UCI)](https://www.kaggle.com/datasets/obeykhadija/drug-consumptions-uci?resource=download).
5. Stephen Few. [Data Visualization Effectiveness Profile](https://www.perceptualedge.com/articles/visual_business_intelligence/data_visualization_effectiveness_profile.pdf).
6. Berinato, Scott. *Good Charts*. Harvard Business Review Press.