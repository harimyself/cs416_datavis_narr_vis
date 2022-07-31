## CS416 Data Visualization: Narrative Visualization
### Author: hbojja2@illinois.edu



#### Summary:
This page was constructed based on the `data-science-job-salaries` dataset from kaggle. The idea is to understand the data science job market between the years 2020 to 2022. For this we have chosen 7 most interesting jobs titles from the full set of 41 different jobs.

The 7 job titles illustrated are listed below in the same order.

##### Job Titles:
1. Applied Data Scientist
2. Data Science Manager
3. Data Scientist
4. Data Specialist
5. Head of Data Science
6. Machine Learning Engineer
7. Machine Learning Scientist

The goal of this narrative visualization is show 
1. Which of 7 Data Science or AI jobs has highest paying salary and in which year? 
2. Which year between 2020-2022 a particular job title has highest salary?



**Years Illustrated:** 2020, 2021, 2022

#### Narrative & Visual Structure:
The visualization follows interactive slideshow designs to illustrate the data. Though the slides are organized in the sorted order of job titles, the viewer has the liberty to click and view the scene in any demanded order.

Viewers can also navigate from one scene to another by using next and previous buttons on the button panel at the bottom of the graph. The Summary button can be used to reset to the default state showing data points for all titles.

All job titles listed above are dynamically extracted from the job salaries csv file. These clickable job titles are listed horizontally on the left side of the visualization. Each title is rendered with a unique color. The same color would be used further to render the data related to that job title.

Upon clicking a job title the scene on the right side of the visualization changes showing the dynamically filtered data for that particular job title. For ease of narration, the data plot rendered for a job title has the same colored data points as the title.

**For Example:** The job `Data Scientist` is rendered in red color. The plot rendered upon clicking the title has the same red colored data points.

##### Scene:
Each scene is a plot with years 2020, 2021, 2022 on x-axis. The salaries are then rendered on y-axis. The data point that appears highest on y-axis considered the maximum salary observed.

The viewer can transition from one scene to another by clicking on the titles listed on left side of the illustration. The plot can also be reset by clicking on `reset` button at the bottom of the graph.

Every scene is smoothly transitions as the salary points start at the top of y-axis slowly moving to their desired locations.

The maximum salary point has also been **annotated with callout circle** to grab viewer's attention. The annotation contains the salray in $ as title and shows the corresponding job title as label.

**For Example:** The default state of the plot shows the Max Salary: $412000 for the job Data Scientist. 

##### Parameters and triggers:
Each job title listed is rendered with unique color for clear distinguishion. The following parameters are captured and transferred to start rendering a scene.

- Job Titles: Job titles change as the viewer clicks on next or prev buttons. The changed value is shown on the top of the scene.
- Color: Distinct colors used to render each job title.
- Transition: A transition of 2000ms is used to move the circular data points from top of y-axis to desired locations.
- Salary: Salary is used on the y-axis of the scene plot.
- Max Salary & Year: Every scene captures the max salary and year parameters specific to that scene.

The page is in default state on load. Viewers could navigate from one scene to another by clicking buttons in the button panel.
Default State: Shows salaries of all job titles across all years. Summary burron can restore the page to this state from any state of scenes.
Title State: This state can be reached either by clicking on job title or next and prev buttons.

##### Triggers:
Next and Prev buttons, each of the job titles used as a trigger to transition from one scene to another.
The data points in the scene plot react by hovering event on top of them. The details of the hovered data point is shown in tooltip.
There is a Summary button at the bottom to trigger the default state.


### Visualization
{% include narr_vis.html max-width="900px" max-height="800px" %}
