---
layout: page
title: Using Trace Data to Find Evidence of Curiosity in Learning
description: Telemetry Data from IFN619 2023
img: assets/img/stay_curious.jpg
importance: 2
category: phd project
---

# Presentation on Week 13

The contents in this section were presented in classes on Week 13. The original contents were migrated from the Google Sites. 
For any updates after the presentation, please go to the next section. 

## Purpose

This was initially a short presentation to the IFN619 class - Semester 1, 2023. The initial purpose of this project page is to inform the students who opted in to provide their Jupyter telemetry data from the IFN619 class. 

If you are a participant of this project, please contact me if you want to know more about this project. 
I will keep updating this project page as I dig more into the telemetry data. 

## A little recap

- Video & participant information sheet on Canvas (see screenshot) 

- My PhD topic is about identifying and supporting curiosity in learning with a data-driven approach.

- Telemetry data from JupyterLab environment is collected. All the data are anonymous. 

- My hypothesis: students behave differently; different patterns will correlate with features signifying curiosity.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/canvas-screenshot.png" title="canvas screenshot" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    At the beginning of the semester, I uploaded a short video and a participant information sheet on Canvas introducing this project. You can find more information under `Module > Data Analytics Research` on Canvas IFN619 page. 
</div>

## What did I propose to do? (More information on the participant information sheet)
During the semester: 

    - Collect and analyse telemetry data only from the studio notebooks
    
    - Data for students from my tutorial sessions are excluded
    
    - Analyses only focus on class level (mainly exploratory analysis - focusing on observing patterns)
    
    - Present a brief overview at the end of the semester (this presentation)

After the final grade is released: 

    - Analyse all the data from the participants
    
    - Insights will be used as the first phase of my PhD project

## Data Overview
### What does the original data look like? 

<div class="row justify-content-sm-center">
    <div class="col-sm-9 mt-3 mt-md-0">
        {% include figure.html path="assets/img/sample-telemetry.png" title="sample telemetry" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-3 mt-3 mt-md-0">
        {% include figure.html path="assets/img/file-size.jpg" title="file size" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

### An overview of the studio notebook data

<div class="l-page">
  <iframe src="{{ '/assets/plotly/fig1.html' | relative_url }}" frameborder='0' scrolling='no' height="500px" width="100%" style="border: 1px dashed grey;"></iframe>
</div>

- Data from 96 out of 98 students (2 students never opened any studio notebooks?)

- Some students were using their local machines. Those students might only use the Jupyter environment to sync notebooks. 

- Wide range of activities by students. Do they have different patterns of using those studio notebooks?

<div class="l-page">
  <iframe src="{{ '/assets/plotly/fig2.html' | relative_url }}" frameborder='0' scrolling='no' height="500px" width="100%" style="border: 1px dashed grey;"></iframe>
</div>

- Most of the events from the top 6 are reflected in the common use of notebooks for general exploration.

- There is a **high rate of errors**. What could be the potential reasons? Are these errors from a few students or all students? What types of errors are common, and are there any variations in the types of errors among students?

- There are **not many "add cell" events**. Is this because students do not need to add new cells for studio notebooks? Who added cells and when did they do so?

- It would be interesting to investigate **copy/cut/paste activities**. Did these activities occur only among some students? Where did they copy and paste the code from?

## Now looking into events for each student...

<div class="l-page">
  <iframe src="{{ '/assets/plotly/fig3.html' | relative_url }}" frameborder='0' scrolling='no' height="500px" width="100%" style="border: 1px dashed grey;"></iframe>
</div>

- Running into errors is quite common for most students.

- It might be able to provide more insights if I standardise each student's activities on the same scale (by looking at the proportion of each event). See below...

- The behavioural patterns might differ depending on whether the notebook is a solution or not. This needs to be examined at the individual level.

### After normalising the events...

<div class="l-page">
  <iframe src="{{ '/assets/plotly/fig4.html' | relative_url }}" frameborder='0' scrolling='no' height="500px" width="100%" style="border: 1px dashed grey;"></iframe>
</div>

- A few students' activity patterns seemed to be different, for example, #185, #190, #188, and #181. 

- It might also be because they didn't use the Jupyter environment as their main platform. 

- This needs to be investigated at the individual level to find out.

## Time Series Data Visualisation - activity frequency on studio notebooks

<div class="l-page">
  <iframe src="{{ '/assets/plotly/fig5.html' | relative_url }}" frameborder='0' scrolling='no' height="500px" width="100%" style="border: 1px dashed grey;"></iframe>
</div>

- Studio notebooks were mostly used during studio sessions (Duh!), and then during tutorial sessions.

- Did student interaction decrease as the semester progressed?

- What activities did students engage in outside of class times? Did they use that time to catch up on content or copy code for assignments?

### What else do I intend to do with studio notebook data?

- Zoom in on the studio sessions and compare them with lecture recordings.

- Identify patterns in student interaction during class and determine when students were most interactive.

- Analyse the data to identify curious behavioural patterns and establish connections between different patterns.

## Next Steps

### More analysis will be done after the semester ends... 

Some explorations were mentioned earlier, such as looking into errors.  

#### More ideas from my pilot analysis... 

Analysing all the data to see when students were more active

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/timeline_week_10_11.png" title="pilot timeline" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/individual_activities.png" title="pilot individual activities" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

- Social network analysis on patterns of behaviours by individual students

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/sna_116.png" title="pilot sna 116" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/sna_127.png" title="pilot sna 127" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

- With new labels for different types of notebooks, I can also investigate how students use different types of notebooks. 

## In the future... 

- Integrate findings from the telemetry data with reflective data.

- Interviews and/or surveys for detailed self-report data. 

---

# A more comprehensive analysis (work in progress)

This section records all the steps I am taking to analyse the telemetry data. Since this is a work in progress, the contents below may not be consistent. I will try to update as much as I can to have a clear flow. Thanks for your understanding. 

## Preparation

I continued to use the code from previous analysis. The first step is to combine all the data into a single file with a tabular format. 
As mentioned above, one activity (such as a click by a student) is recorded as a single `JSON` file, including the event and many information associated with the event. 
Since there are around **7.7 millions** of files, it will take a long time to process all the data. However, I only extracted the information I consider to be important to my study at this stage, including `event_name`, `session_id`, `session_seq`, `request_time`, `user_id`, `error_name`, `error_value` and `notebook_name`. Below is a short description of those variables:

- `event_name`: The name of an event from a student interacting with the Jupyter Notebook. 14 events are recorded in the data: 
    - open_notebook
    - close_notebook
    - save_notebook
    - notebook_visible
    - notebook_hidden
    - scroll
    - cell_executed
    - active_cell_changed
    - add_cell
    - remove_cell
    - cell_errored
    - clipboard_copy
    - clipboard_paste
    - clipboard_cut
- `session_id`: Every time a student opens a Jupyter Notebook triggers a "session". If a student opens multiple notebooks in the Jupyter environment, multiple sessions will be generated. 
- `session_seq`: Each event within a session is assigned a session sequence. Since a student can open multiple notebooks, resulting in multiple sessions recorded simultaneously. Therefore, we consider session sequences as a linear process. 
- `request_time`: Timestamp of the event occurred. All the time are UTC time. Later, I will convert the time into Brisbane time to align with the class times. 
- `user_id`: In the raw data, `user_id` is the QUT student ID. As part of the ethical considerations, I will not use `user_id` as the unique identifier. I will replace the `user_id` with randomly generated ID numbers so student identities remain unrevealed. Please note, only `open_notebook` event files recorded `user_id`, therefore, I have to use `session_id` to link all other events to the same user. 
- `error_name`: Events only recorded when an error is occurred in a Jupyter Notebook. 
- `error_value`: The error message displayed when an error is occurred. 
- `notebook_name`: This is the new feature this semester. It records the name of the Jupyter Notebook the event was triggered. Recording the notebook names is important for my project as different types of events may associated with different types of notebooks. For example, for a studio notebook, students may follow the steps of a lecture and fill the gaps as they listen to the lecture; for a tutorial notebook, students will try some code by themselves. Therefore, you would imagine the majority of events for a studio notebook will be executing cells, while a tutorial notebook will have a wider variety of events such as copying, pasting, running into errors, etc. This example is only considering the scenario during a learning experience by a student, it may change when assignments involved.

After over 2 hours, all the raw data have been processed into a single csv file for cleaning and processing. 

## Data preparation

It is not too bad to reduce the size from the raw data (~250 GB) to the processed csv file (~750 MB). The raw data contains 7,685,002 rows of records. Below are some statistics and initial observations about the raw data:

- Observations on events:
  - The most frequent event is `scroll`. Top 3 also includes changing active cells and executing cells. This is expected as those three events are the most common activities when a user is using Jupyter Notebook.
  - The least frequent events are closing notebooks and clipboard cut. This also makes sense, as users tend not to close their notebooks when they finish using the Jupyter environment (but they will remember to save their notebooks). They also tend to use "copy" instead of "cut" when getting information from one location to another. 
  - More "clipboard paste" events than the combination of "clipboard copy" and "clipboard cut". More likely students copied information from other resources such as the Internet. 
  - Lots of errors occurred when using Jupyter notebooks (Top 4!). 
- Observations on sequences:
  - How long a student stayed within a notebook during a session varied significantly. The average events per session is 537.633, but the standard deviation is 833.919. The median is 243 but the max is 9865. 
  - The statisitics above doesn't really mean anything as one person can have multiple sessions simultaneously. In addition, depending on what kind of notebooks, for example, students may spend more time in a session on their assignment notebook, and they might just open one studio notebook to quickly grab some information. 
- Events from 194 users are recorded. Please notes the teaching team and administrators are also included in the data. Those data will be removed during the data cleaning process. 
- Observations on errors:
  - 80 different types of errors occurred in the data. The top 5 errors are: `NameError`, `SyntaxError`, `KeyError`, `ValueError` and `TypeError`. All those "popular" errors seem to be quite common in using Jupyter notebooks, particularly for Python beginners. 
  - As mentioned above, errors took place very frequently in the records. Dig into how different students deal with errors might be beneficial to study curiosity. 
- Observations on notebook names:
  - Not surprisingly, most events were generated in the assignment notebooks. Students generated also doubled amount of events in assignment 1 than in assignment 2. 
  - Students also spent a large amount of time on notebooks generated by themselves (as shown `NaN`). 
  - More events were generated in the notebooks from earlier weeks of the semester, indicating students might have tended to spend more time studying in the beginning of a semester. However, since the notebooks from earlier the semester were released early, we also need to consider the length of "availability" to students. So we cannot really make that statement that students spending more time in the beginning of the semester.
  - Surprisingly, students tended to spend more time on studio notebooks than tutorial notebooks. The least visited notebooks are the solutions. 

Above information may not be accurate because there are lots of issues in the raw data. The next step will be clean the data and some exploratory data analysis as data cleaning progresses.

## Data cleaning

Steps as listed below were taken to clean the data:

- As mentioned earlier, only files from `open_notebook` events recorded the `user_id`. In addition, `open_notebook` events are the first event of each session, therefore, it always shows as 0 in the `session_seq`. Each session was automatically assigned a `session_id`. The first step is to fill the `na` values from the `user_id` column based on the `session_id` information.
- Once all the users were identified in the dataset, I then replaced the real IDs with some computer-generated IDs. Therefore, no student identities can be identified from the analysis. 
- Since nobody opted out from the experiment, no action was taken to remove any records from the dataset. 
- During the semester, a filter was applied to only include the studio notebooks in the analysis. The studio notebooks can be identified by the `notebook_name` column. Since the semester for IFN619, semester 1 concluded, this filter does not need to be applied for the analysis. 
- Note that the student list was from week 3, therefore, if any students who enrolled after week 3 were not included in the analysis (as proposed in the ethics application). In addition, some students might drop out of the unit after week 3. For those students, I will apply a filter to check when was their last activity in the Jupyter environment. No further activities after the census day are considered to be inactive and will not be included in the analysis. There were 189 users in the Jupyter environment, including teaching staff and students who dropped out before week 3. After adding the filter of week 3 list, 178 students were included in the dataset. The next step is to remove inactive students. 
- In order to compare dates, I need to convert `request_time` column to a datetime data type. I have also convert the datetime to Brisbane time as the original `request_time` used UTC time. The new column is named as `datetime_bne`. 
- Based on the filter, 4 students dropped out of this unit before the census day. 4 students dropped out of this unit after the census day, before the first assignment is due. 1 student dropped out right before the date for "withdraw without an academic panelty". Those students were not included in the analysis, therefore, **data from a total of 169 students will be included in the analysis**. 

