+++
title = "Slides"
slug = "slides"
+++

This weekly slides updating program was made by me during my internship at Trina. It was mainly used for weekly usage during the internship. However, I am now looking to add an email component to the program, both for crawling for new links (some links are updated monthly and are tracked down by my coworker), as well as automating sending an updated slide to them.

### Github
https://github.com/stevenzhujr/Slides

### Abstract

The main goal of this project was to write a program that would update slides weekly. I used python and its various libaries to fetch the needed elements from the web, treat them, and then update the slides.

### Parts

**Webfetch**: Using Selenium, I could open browsers remotely. This allows me to then use XPath to find the element, and take a screenshot of said element or take in its value. However I found that some websites had ads that would block the elements that I needed. To remedy this, I added a plugin that would be installed when the browser is launched. Once launched, the browser would wait 5 seconds so that it ise in effect, then capture the elements.

**Treatment**: Using the pillow library, I edit the screenshots I get from the web. This is due to the fact that not all the screenshots I need correspond to its web element completely.

**Clear**: Using the pptx libary, I clear the slide and prime it for editing.

**Update**: Using the pptx libary, I update the slide so that it is upd to date. I use runs within paragraphs so that I can format the text boxes customly.

### In action
{{< vimeo_simple "872103863?share=copy" >}}