---
layout: page
title: Using Trace Data to Find Evidence of Curiosity in Learning
description: Telemetry Data from IFN619 2023
img: assets/img/stay_curious.jpeg
importance: 1
category: phd project
---

# Purpose

This was initially a short presentation to the IFN619 class - Semester 1, 2023. The initial purpose of this project page is to inform the students who opted in to provide their Jupyter telemetry data from the IFN619 class. 

If you are a participant of this project, please contact me if you want to know more about this project. 
I will keep updating this project page as I dig more into the telemetry data. 

# A little recap

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

# Data Overview
## What does the original data look like? 

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/sample-telemetry.png" title="sample telemetry" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/file-size.jpg" title="file size" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

## An overview of the studio notebook data

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

# Now looking into events for each student...

<div class="l-page">
  <iframe src="{{ '/assets/plotly/fig3.html' | relative_url }}" frameborder='0' scrolling='no' height="500px" width="100%" style="border: 1px dashed grey;"></iframe>
</div>

- Running into errors is quite common for most students.

- It might be able to provide more insights if I standardise each student's activities on the same scale (by looking at the proportion of each event). See below...

- The behavioural patterns might differ depending on whether the notebook is a solution or not. This needs to be examined at the individual level.

## After normalising the events...

<div class="l-page">
  <iframe src="{{ '/assets/plotly/fig4.html' | relative_url }}" frameborder='0' scrolling='no' height="500px" width="100%" style="border: 1px dashed grey;"></iframe>
</div>

- A few students' activity patterns seemed to be different, for example, #185, #190, #188, and #181. 

- It might also be because they didn't use the Jupyter environment as their main platform. 

- This needs to be investigated at the individual level to find out.

# Time Series Data Visualisation - activity frequency on studio notebooks

<div class="l-page">
  <iframe src="{{ '/assets/plotly/fig5.html' | relative_url }}" frameborder='0' scrolling='no' height="500px" width="100%" style="border: 1px dashed grey;"></iframe>
</div>

- Studio notebooks were mostly used during studio sessions (Duh!), and then during tutorial sessions.

- Did student interaction decrease as the semester progressed?

- What activities did students engage in outside of class times? Did they use that time to catch up on content or copy code for assignments?

## What else do I intend to do with studio notebook data?

- Zoom in on the studio sessions and compare them with lecture recordings.

- Identify patterns in student interaction during class and determine when students were most interactive.

- Analyse the data to identify curious behavioural patterns and establish connections between different patterns.

# Next Steps

## More analysis will be done after the semester ends... 

Some explorations were mentioned earlier, such as looking into errors.  

### More ideas from my pilot analysis... 

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
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/sna_116.png" title="pilot sna 116" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/sna_127.png" title="pilot sna 127" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

- With new labels for different types of notebooks, I can also investigate how students use different types of notebooks. 

# In the future... 

- Integrate findings from the telemetry data with reflective data.

- Interviews and/or surveys for detailed self-report data. 
