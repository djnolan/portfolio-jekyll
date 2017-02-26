---
layout: project
title: Anatomy of an Exodus
date: 2016-12-22
date_text: December 22
date_year: 2016
thumbnail: exodus_th.jpg
thumb_alt: Graphics showing the number of migrant arrivals to Greece and Italy in 2015.
include: exodus
view_site: http://apps.frontline.org/anatomy-of-an-exodus/
roles: 
 - user experience
 - visual design
 - HTML/CSS
 - data/reporting
---

[Anatomy of an Exodus](http://apps.frontline.org/anatomy-of-an-exodus/) is a visual story that explains the European refugee crisis through maps and data graphics. The experience was driven by data from the beginning. First, I gathered reliable sources that would provide detailed monthly and up-to-date data we would need to break down the crisis. The story covers the peak of the refugee and migrant arrival to Europe in 2015, the response from EU countries and the status of the crisis at the end of 2016. Digital reporter [Priyanka Boghani](https://twitter.com/priyankaboghani) shaped the narrative, wrote the text and provided an overall expertise on the subject that helped shape the design throughout.

This is a visual explainer—big images with very little text. At FRONTLINE, we tend to embrace scrolling experiences for nearly every custom interactive, but in this case I thought a fullscreen slideshow approach would provide the right container to shape a story driven by visuals.

## The Container
We went with [swiper js](http://idangero.us/swiper/#.WKCKSWQrK2x) to power the slideshow. It provided a flexible, blank canvas to start from with built-in gestural behaviors for mobile touch. We were careful to tailor some interactions for the unique capabilities of devices. The desktop experience uses left/right arrows for navigation with additional keyboard controls. On mobile we encourage swiping with an initial instruction and we decided to keep the left/right arrows as a fallback in case the user prefers that interface. 

We chose a horizontal slide transition. We found that a vertical transition came with the dangers of scroll jacking if not implemented perfectly.

In this case the fullscreen slider experience was a nice alternative to scrolling because the graphics and captions broke up into small sections that fit within view across devices (more on this later).

## The Charts
{% include inline-wide-split.html inline_img1='exodus_arrivals.jpg' inline_img2='exodus_applications.jpg' alt1='Monthly arrivals to Europe by sea, 2014 and 2015.' alt2='2.2 million asylum applications to the EU, 2015–2016.' %}

The charts are all svg images with html text labels and headings. Most are made using [ai2html](http://ai2html.org/) as a starting point to generate a responsive html chart from an illustrator file. I broke down the data into digestible chunks to visualize on each slide. Each chart needed to be robust enough to stand on its own, but simple enough to be scaled down to fit on the smallest device and stay in view.

## The Maps
{% include inline-wide.html inline_img='exodus_greece.jpg' alt='Map showing migrant arrivals to Greek islands in 2015.' %}

I wanted the maps to provide a striking textural contrast to the flat charts. I needed high resolution satellite imagery to show details of small islands and I wanted the terrain to reinforce the fact that migrants are making a journey across varied and sometimes dangerous land and water. After looking into several map resources I found that [NASA Visible Earth](http://visibleearth.nasa.gov/) had the best quality images with the most reliable and well-documented information. I used [Natural Earth](http://www.naturalearthdata.com/) vector data and changed the projection in [QGIS](http://www.qgis.org/en/site/) to match the projection of the satellite image. The final step was to manually delete the outer country vector borders that touch water, because the contrast between water and land in the satellite image makes for a stronger and more natural separation.

## The Small Screen
{% include inline-wide-fourths.html inline_img1='exodus_arrivals_m.png' inline_img2='exodus_italy_m.jpg' inline_img3='exodus_origin_m.png' inline_img4='exodus_deaths_m.png' alt1='Monthly arrivals to Europe by sea, 2014 and 2015. Graphic shows the mobile screens layout.' alt2='Map showing migrant arrivals to locations in Italy in 2015. Graphic shows the mobile screens layout.' alt3='Migrant arrivals to Greece and Italy in 2015, showing country of origin. Graphic shows the mobile screens layout.' alt4='Mediterranean deaths in 2015 and 2016. Graphic shows the mobile screens layout.' %}

Making all the graphics fit within the height of the smallest devices with minimal or no scrolling was difficult to do here. Most of the graphics fit on screen on the smallest devices but there is some overflow scrolling to accommodate additional data notes and credits.

## The Data
{% include inline-col.html inline_img='exodus_deaths.jpg' alt='Mediterranean deaths in 2015 and 2016.' %}

I’m a graphic designer and interactive designer at heart—journalism is still new to me. That being said, I took the lead in gathering all the data and figuring out what story we could tell with it. This allowed me to gain a deeper knowledge of the data and content overall so I could plan out the experience more confidently and visualize each piece knowing exactly how everything fit together.

