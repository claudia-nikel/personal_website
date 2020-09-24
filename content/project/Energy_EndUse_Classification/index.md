---
title: Energy End-Use Classification
summary: For my Capstone project I helped create a python program that queries live streaming sensor data from the UDL SkySpark database, cleans and uses appropriate Machine Learning methods to apply NRCan Secondary End-Use Classifications to the data
tags:
- python
- classification
- Data Science
- Interactive Visualizations
date: "2020-05-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
Project_Website: "https://urbandatalab.io/project/mds-captone-2020/"

image:
  caption: Overview of Project Solution
  focal_point: Smart

links:
url_code: "https://urbandatalab.io/project/mds-captone-2020/"
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---

The end-use classification model was written in the Python language and makes use of common packages used for data wrangling, analysis, and modeling such as Pandas and Sci-Kit Learn. The general concept is shown in the flowchart below.

<p align="center"><img src="/img/CapstoneProgramFlowChart.png" alt="CapstoneProgramFlowChart" width="200"/></p>

<br/>

# About the Model
The basic idea is to first condense the ~7800 NC sensors in the Pharmacy building down to a more manageable size using clustering. Next, model and extract information on how these clusters of NC sensors react relative to each EC sensor. Finally, pass the numbers representing that relationship between NC and EC sensors into a supervised classification model along with some other information about the EC sensors and a “training” set of EC sensors that have already been manually labelled with end-use types. Once this model has been trained on this set of EC sensors, it can be used to predict end-uses for data without known end-uses and the results can be stored back into UDL’s InfluxDB instance. Please see the project’s GitHub repository for a full report and more details on the model.



<p align="center"><img src="/img/maRs_wind_speed.png" alt="maRs_temperature" width="200"/></p>

Link to project repository: https://github.com/UBC-UrbanDataLab/Classifying-End-Use-MDS2020 <br/>
Link to project on companies website: https://urbandatalab.io/project/mds-captone-2020/ <br/>
Co-collaborator: Eva Nguyen, Connor Lee, Alex Tamm
