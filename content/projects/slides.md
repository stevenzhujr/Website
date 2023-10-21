+++
title = "Slides"
slug = "slides"
+++

This weekly slides updating program was made during my internship at Trina.

### Github
https://github.com/stevenzhujr/Slides

### Abstract

The main goal of this project was to write a program that would update slides automatically on weekly basis. I used python and its various libraries to fetch the needed elements from the web, process them, and then update the slides.

### The code is composed of the following parts:

**Webfetch**: Using Selenium, I could open browsers remotely. This allows me to use XPath to find the web element, take a screenshot of appropriate element or take in its value. 

However some websites had ads that may block the elements needed. To remedy this, I used Selenium to automatically inatall an adblocker plug in before capturing the elements.

**Treatment**: Sometimes not all the screenshots from the web were properly captured. With Pillow library I can edit the screenshots. 

**Clear**: With PPTX library I can clear the slide and prepare it for editing.

**Update**: With the PPTX library I can update the slide with new information. I use runs within paragraphs so that I can format the customary text boxes.

### In action
{{< vimeo_simple "872103863?share=copy" >}}