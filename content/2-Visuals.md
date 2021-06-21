---
title: Visuals
nav: Visuals
topics: Template; Config; Lorem ipsum
---

## Visualisations

We now explore some examples of visualisations. Be aware there are so many possibilities out there for visualising your data. Think beyond the standard line or bar graphs!

### Visualise your thesis
Visualise Your Thesis (https://library.unimelb.edu.au/research/visualise-your-thesis#resources) is an international competition run by the University of Melbourne that challenges Higher Degree by Research (HDR) students to summarise their research in an engaging, 60-second visual presentation using a supplied template, that encapsulates your research project. It gives you the opportunity to build essential digital communication skills so you can effectively communicate complex research to a general audience. Competition submissions are judged on their visual impact, and how well the content presents the research. The competition allows for multi-media, interactivity and interpretation and is suitable for all disciplines. The video here is from a 2019 winner, HDR student at UTS.
youtubeid: Am-AvhPl0jA

### Video timelapse
You can highlight that time lapses would work well for event set ups, constructing buildings, or use of infrastructure throughout a day. This Pea Shoot video is very peaceful and therapeutic. 
youtubeid: w77zPAtVTuI

### Google Earth Timelapse
Earth Timelapse is a global, zoomable video that lets you see how the Earth has changed.
https://earthengine.google.com/timelapse/

### Interactive graphs
This new York Times' swing history graph really impressess audience.
"image/Swing_State.png"

This word cloud is developed from Shakespeare masterpieces.
"image/Word_Cloud.png"


Edit the `_config.yml` to get your workshop website set up with the basics such as `title` and `author`.
Check comments in the file for all the options!

Once you have edited the `_config.yml`, you are ready to start editing your content pages.

## Advanced Options [optional]

### Using figure include

- put any images you want to use in the "images" folder.
- in a markdown file where you want the image to appear, use the `figure.html` include on its own line, following the pattern: `{% include figure.html img="my-cat.jpg" alt="cat" caption="My cat" width="50%" %}`
- figures will be centered, and can optionally be given a caption and percentage width.

Additional includes are available in the "_includes" folder, check the comments for how to use them (or see the next lesson page for demos).

### Basic style customization

- the `custom.scss` in the `assets/css` folder exposes variables that can customize the basic style of website.
- Give a tiny splash of color on the header and footer borders by tweaking the `$top-border` 
- `$link-color` colors links

### Add Optional Analytics

- To use Google Analytics, add your analytics id to `_config.yml` in `google-analytics-id:` (if `google-analytics-id` is blank, the GA code will not added)
- To use an alternative analytics, paste the code snippet provided by the platform into `_includes/template/analytics.html`
- analytics code will only be added when using "production" environment. This happens automatically on GitHub Pages. To build manually you need to add "JEKYLL_ENV", like: `JEKYLL_ENV=production jekyll build`