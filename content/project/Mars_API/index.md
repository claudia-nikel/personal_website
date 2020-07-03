---
title: Mars API
summary: A `Mars_API` to retrieve and visualize weather data from the last 7 Sols (Martian days) as recorded and updated daily by NASA’s InSight Mars lander. InSight is located at Elysium Planitia, a flat surface near the equator of Mars.
tags:
- API
- Data Science
date: "2020-01-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
Mars_API: "https://github.com/claudia-nikel/maRs "

image:
  caption: Photo of temperature gauge
  focal_point: Smart

links:
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example
---

An API to retrieve and visualize weather data from the last 7 Sols (Martian days) as recorded and updated daily by NASA's InSight Mars lander. InSight is located at Elysium Planitia, a flat surface near the equator of Mars. The python package built contains four functions: 
<br/>

`marsInfo`: returns a summary table of weather including the Sol number, datetime stamp of first recorded sample (`First_UTC`), last recorded sample (`Last_UTC`), the current season for Mars, as well as average (`av`), sample size (`ct`), minimum (`mn`) and maximum (`mx`) recordings for temperature (`AT`), horizontal windspeed (`HWS`), and pressure (`PRE`). <br/>

`marsAverage`: takes the saved output from the marsInfo() function and returns the average temperature, windspeed, and pressure for the last 7 Sols.

`windspeed`: retrieves the inputted Sol's horizontal wind speed (m/s) from the summary table and visualizes it as a dial. The black bar is the average windspeed for the Sol, which corresponds to the black text. The green background is the sol range (min and max), and the red or green text below is represents a decrease or increase, respectively, relative to the previous sol's average. <br/>


`pressure`: retrieves the inputted Sol's pressure (Pascal) from the summary table and visualizes it as a dial. The black bar is the average pressure for the Sol, which corresponds to the black text. The orange background is the sol range (min and max), and the red or green text below is represents a decrease or increase, respectively, relative to the previous sol's average. <br/>

`temperature`: retrieves the inputted Sol's temperature (converted from Farhenheit to degrees Celsius) from the summary table and visualizes it as a dial. The black bar is the average temperature for the Sol, which corresponds to the black text. The blue background is the sol range (min and max), and the red or green text below is represents a decrease or increase, respectively, relative to the previous sol's average. <br/>
