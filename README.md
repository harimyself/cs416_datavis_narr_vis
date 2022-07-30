## CS416 Data Visualization: Narrative Visualization
### Author: hbojja2@illinois.edu



#### Summary
This page was constructed based on the `data-science-job-salaries` dataset from kaggle. The idea is to understand the data science job market between the years 2020 to 2022. For this we have chosen 7 most interesting jobs titles from the full set of 41 different jobs.

The goal of this narrative visualization is show 
1. Which of 7 Data Science or AI jobs has highest paying salary and in which year? 
2. Which year between 2020-2022 a particular job title has highest salary?

The 7 job titles illustrated are also listed below in the same order.

##### Job Titles
1. Applied Data Scientist 
2. Data Science Manager 
3. Data Scientist 
4. Data Specialist 
5. Head of Data Science 
6. Machine Learning Engineer 
7. Machine Learning Scientist

##### Years Illustrated: 2020, 2021, 2022


#### Narrative & Visual Structure.
The visualization follows `interactive slideshow` designs to illustrate the data.

All job titles listed above are dynamically extracted from the job salaries csv file. These `clickable job titiles` are listed horizontally on left side of the visualization. Each title is rendered with a unique color. The same color would be used further to render the data related to that job title.

Upon clicking a job title the scene on right side of the visualization changes showing the dynamically filtered data for that particular job title. For ease of narration, the data plot rendered for a job title has the same colored data points as the title.

##### For Example: 
The job `Data Scientist` is rendered in red color. The plot rendered upon clicking the title has the same red colored data points.

##### Scene
Each scene is a plot with years 2020, 2021, 2022 on x-axis. The salaries are then rendered on y-axis. The data point that appears highest on y-axis considered the maximum salary observed.

The maximum salary point has also been annotated / highlighted with `callout circle` to grab viewer's attention.

The viewer can transition from one scene to another by clicking on the titles listed on left side of the illustration. The plot can also be reset by clicking on `reset` button at the bottom of the graph.


{% include narr_vis.html max-width="850px" max-height="800px" %}

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/harimyself/cs416_datavis_narr_vis/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
