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
The visualization follows `interactive slideshow` designs to illustrate the data. The design lets the viewer access the scenes in any order the viewer chooses.

All job titles listed above are dynamically extracted from the job salaries csv file. These `clickable job titiles` are listed horizontally on left side of the visualization. Each title is rendered with a unique color. The same color would be used further to render the data related to that job title.

Upon clicking a job title the scene on right side of the visualization changes showing the dynamically filtered data for that particular job title. For ease of narration, the data plot rendered for a job title has the same colored data points as the title.

**For Example: ** The job `Data Scientist` is rendered in red color. The plot rendered upon clicking the title has the same red colored data points.

##### Scene:
Each scene is a plot with years 2020, 2021, 2022 on x-axis. The salaries are then rendered on y-axis. The data point that appears highest on y-axis considered the maximum salary observed.

The viewer can transition from one scene to another by clicking on the titles listed on left side of the illustration. The plot can also be reset by clicking on `reset` button at the bottom of the graph.

Every scene is smoothly transitions as the salary points start at the top of y-axis slowly moving to their desired locations.

The maximum salary point has also been **annotated with callout circle** to grab viewer's attention. The annotation contains the salray in $ as title and shows the corresponding job title as label.

**For Example:** The default state of the plot shows the Max Salary: $412000 for the job Data Scientist. 

##### Parameters and triggers:
Each job title listed is rendered with unique color for clear distinguishion. The following parameters are captured and transferred to start rendering a scene.
- **Job Titles:** Job titles listed above act as the triggers to transition from one scene to another.
- **Color:** Distinct colors used to render each job title.
- **Transition:** A transition of 2000ms is used to move the circular data points from top of y-axis to desired locations.
- **Salary:** Salary is used on the y-axis of the scene plot.
- **Year:**: Year of the recorded 

Each of the job title used as trigger to transition from one scene to another. The data points in the scene plot react for hovering on top of them. The details of the hovered data point are shown in tooltip. There is an **Reset** button at the bottom to trigger the default state.

The highlight of the transition is that the scenes can be accessed in any order.

### Visualization
{% include narr_vis.html max-width="900px" max-height="800px" %}

