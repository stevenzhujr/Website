+++
title = "(9/2022) Weekly Updating Slides"
slug = "slides"
+++

The Weekly Slides Automation Project was made during my internship at Trina.

### Github
https://github.com/stevenzhujr/Slides

### Abstract

The main goal of this project was to write a program that would update slides automatically every week. I used Python and its various libraries to fetch the needed elements from the web, process them, and then update the slides.

### The code is composed of the following parts:

**Webfetch**: Using Selenium, I could open browsers remotely. Allowing me to use XPath to find the web element and either take a screenshot of it or record its value. 

However, some websites had ads that may block the screenshots needed. To remedy this, I used Selenium to automatically install an adblocker plug-in before capturing the elements.

**Treatment**: On occasion, not all the screenshots were captured in the necessary dimensions. With the Pillow library, I can edit the screenshots. 

**Clear**: With the PPTX, library I can clear the slide and prepare it for editing.

**Update**: With the PPTX, library I can update the slide with new information. I used runs within paragraphs to format the customary text boxes.

### Demo
{{< vimeo_simple "872103863?share=copy" >}}