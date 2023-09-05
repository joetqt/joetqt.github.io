---
layout: page
title: Confidence and Curiosity 
description: Telemetry Data from IAB303 2023
img: assets/img/banner-typing.jpg
importance: 1
category: phd project
---

# Introduction on Week 1

The video below was presented in Week 1. This video is also available on Canvas. Please refer to the participant information sheet on Canvas for more details.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="https://www.youtube.com/embed/iZ4fDYZHXb8" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

# Week 2 learning check-in data

*Note: The following information was as accurate as on  2023-08-08 10:45:52 (the last activity in the dataset after syncing).*

On week 2, learning check-ins were embedded in the studio notebook. Students were encouraged to check in at 4 points of time during the studio session with the lecturers. After syncing the data on 2023-08-08, here is some general information I found (**before cleaning the data** - so the data might not be as accurate, but will give you some idea about the data): 

- There are 4 check-ins in the notebook. 
- Data for 123 students were recorded. >> We have 142 students enrolled, which means 19 students haven't even used the Jupyter environment. 
- 56 students completed at least 1 check-in. >> Less than half of the students used the check-in function :'(
- Most students were confident - as most students had a mean confidence level above 8.
- 13 students completed at least 4 check-ins. The majority checked in 3 times. 25 students checked in once or twice. However, at this stage, not all check-ins are genuine. I need to do more data cleaning.


## Check-ins during Week 2 studio sessions

This is the first experience of student learning check-in. The information below only used the data from week 2's studio notebook and included the activities during the studio session (Monday morning 9:00 am - 11:00 am). Later, I may check the data again and I may include data from outside the studio session time. The new data may provide some information about students who watched the recordings or attempted the tasks by themselves outside the studio session time. :

- 34 students checked in at least once during the live studio sessions. 
- Only 4 students completed all 4 check-ins during the studio session. 
- In general, students were quite confident about their learning for the session, as the mean confidence levels for a majority of students were above 7.  
- By roughly observing individual inputs, there were not many changes in the confidence levels during the session. This might be because there were not enough check-ins for the session to show some patterns. 

<div class="l-page">
  <iframe src="{{ '/assets/plotly/fig_303_wk2_mean_conf_studio.html' | relative_url }}" frameborder='0' scrolling='no' height="400px" width="100%" style="border: 1px dashed grey;"></iframe>
</div>

<div class="l-page">
  <iframe src="{{ '/assets/plotly/fig_303_wk2_checkin_count_studio.html' | relative_url }}" frameborder='0' scrolling='no' height="450px" width="100%" style="border: 1px dashed grey;"></iframe>
</div>

Potential issues that need to be solved:

- Some students ran the check-in code in other notebooks
- One student ran 4 check-ins within 2 minutes

What else to do:

- Visualise the confidence levels of each participant
- Modelling confidence levels
- A more close examination of the time spans for check-ins 
- Adding students who checked in outside the studio session

# Week 7 observations

Data was synced in the morning of 2023-09-05. The latest record in this sync was 2023-09-04 22:37:18. 

Quick notes on the data:
- Now we have 140 students in the dataset. Changed from 123 on week 2. 
- Among all the 140 students, 101 students have completed at least 1 check-in.
- Among all the data, several students have an average of 10 out of 10 for their check-ins. 
- In general, the average confidence level for most students were reasonably high (above 5). Only a few students had an average confidence level below 5.
- For the last 7 weeks, we have 3 sessions with check-ins: Week 2, Week 4 and Week 7. The maximum number of check-ins should be 13. Based on all the data, majority students who checked in less than 12 times. However, 14 students checked in more than 13 times. 

<div class="l-page">
  <iframe src="{{ '/assets/plotly/fig_303_checkin_count_all.html' | relative_url }}" frameborder='0' scrolling='no' height="400px" width="100%" style="border: 1px dashed grey;"></iframe>
</div>

## Before looking into week 7 data, let's start with week 4

Instead of looking for only live studio sessions, let's start by looking for the whole week. So it potentially includes students who checked in outside the studio sessions. 

- 111 students logged into the Jupyter environment on week 4. 
- 76 students checked in at least once during the week.
- The majority of students who checked in this week had a mean confidence level above 6. 8 students had a mean confidence level below 6, one student was 1.6.
- 5 check-ins in the notebooks for this week. The majority checked in 5 or less times. 16 students checked in more than 5 times. 

During studio sessions only:
- 60 students logged into the Jupyter environment during the studio sessions.
- 53 of them checked in during the studio sessions.
- Similar patterns than the whole week data. 8 students had a mean confidence level below 6, one student was 1.6. [CHECK] Are they the same students? 
- 5 check-ins in the notebooks for this week. The majority checked in 5 or less times. 9 students checked in more than 5 times. 

<div class="l-page">
  <iframe src="{{ '/assets/plotly/fig_303_wk4_mean_conf_studio.html' | relative_url }}" frameborder='0' scrolling='no' height="400px" width="100%" style="border: 1px dashed grey;"></iframe>
</div>

<div class="l-page">
  <iframe src="{{ '/assets/plotly/fig_303_wk4_checkin_count_studio.html' | relative_url }}" frameborder='0' scrolling='no' height="450px" width="100%" style="border: 1px dashed grey;"></iframe>
</div>


## Week 7 data

Since this is still at the beginning of Week 7, so I am going to look at the check-ins during the live studio sessions only. 

During studio sessions only:
- 49 students logged into the Jupyter environment during the studio sessions.
- 44 of them checked in during the studio sessions.
- Similar patterns from previous weeks. 6 students had a mean confidence level below 6, one student was 2.2. 
- 4 check-ins in the notebooks for this week. Almost half of the students (n=20) checked in more than 4 times. 

<div class="l-page">
  <iframe src="{{ '/assets/plotly/fig_303_wk7_mean_conf_studio.html' | relative_url }}" frameborder='0' scrolling='no' height="400px" width="100%" style="border: 1px dashed grey;"></iframe>
</div>

<div class="l-page">
  <iframe src="{{ '/assets/plotly/fig_303_wk7_checkin_count_studio.html' | relative_url }}" frameborder='0' scrolling='no' height="450px" width="100%" style="border: 1px dashed grey;"></iframe>
</div>

