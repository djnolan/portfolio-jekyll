---
layout: project
title: FRONTLINE Redesign
date: 2015-11-30
date_text: November 30
date_year: 2015
thumbnail: fl_editorial_2.jpg
thumb_alt: 
include: frontline-redesign
view_site: https://www.pbs.org/wgbh/frontline/
roles: 
 - design lead
 - user experience
 - visual design
 - prototype HTML/CSS
---

In 2015, I worked on the redesign of the FRONTLINE website at WGBH Digital. FRONTLINE is the PBS investigative journalism and documentary series. The website has over 200 full films, text articles and interactive features.

I was the lead designer on the project, responsible for the visual design and user experience. Our goals were these: Give the site a visual refresh so it falls more in line with a fresh vision for the FRONTLINE brand. Make it responsive, of course, and optimize the reading and watching experience for mobile. And design to accommodate some unique editorial and publishing processes.

Early on our team worked together to gather user research based on site analytics and a user survey of the existing FRONTLINE audience. We then created user personas and scenarios so we could start to craft our initial solutions to target these specific audiences and use cases. For example, we wanted to target a younger audience coming to our site from facebook that was possibly unfamiliar with FRONTLINE. How could we engage them with a single piece of reporting and then introduce them to a bigger archive of investigative journalism videos and articles? It's scenarios like these that helped shape our initial process and keep the design solutions focused.

## Concept

The FRONTLINE editorial team had specific needs around publishing content. They needed article templates that could accommodate both shorter, quick-hit stories and longer investigative pieces. They wanted to curate and bundle content around film topics. And they had a sometimes infrequent publishing schedule, different from the day-to-day churn of a daily news site. 

My approach: sketch out a loose system of flexible components based on these needs. Our team could then work together to iron out the details of the components and then assemble them together into page templates. All the pages on the site would simply be different configurations of components pulled from the same library.

{% include inline-wide.html inline_img='component_sketches.jpg' alt='' %}

We cut these component sketches out individually and started assembling them into pages. This formed the basis of the site and helped the team get on board with the idea of a website as a system of components and templates. 

Alongside this work our team also began a phase of content strategy that started with an inventory of existing content types. This allowed us to start making decisions around which types of content to prioritize for the redesign and what could be left behind in a legacy format. 

## Wireframes and Prototypes

The success of the paper components lead me to propose a similarly flexible and collaborative method for wireframing. I created rough, responsive html wireframes of individual components. I then could easily assemble the components together in different ways to come up with template variations. All of these initial components and templates were immediately viewable on the devices of team members. We were judging these early design decisions in the right context, the same context where the final website would be seen.

{% include inline-wide-fourths.html inline_img1='component_wires_1.jpg' class1='border' inline_img2='component_wires_2.jpg' class2='border' inline_img3='component_wires_3.jpg' class3='border' inline_img4='component_wires_4.jpg' class4='border' alt1='' alt2='' alt3='' alt4='' %}

Our front-end developer even created a template builder that allowed all members of the team to select components and assemble them into templates. [MAYBE DON'T NEED THIS?]

## User Experience Considerations

We took a deeper look through existing user paths through the site and teased out some flows we wanted to focus on. We wanted to make sure our system of components could be arranged in a way that it would engage the users from our target scenarios and then push them to the right places on our site.

{% include inline-wide-split.html inline_img1='redesign_ux_1.png' inline_img2='redesign_ux_2.png'  class1='border' class2='border' alt1='' alt2='' %}

We refined our components and I created low fidelity static wireframes as a way of documenting the component with it's accompanying rules. (may need to explain what the rules are if the image does not do that)

{% include inline-wide-split.html inline_img1='component_document.jpg' inline_img2='redesign_wire.png' width='thin' class='mobile' class1='border' alt1='' alt2='' %}

## Visual Design

We asked the FRONTLINE team to come up with words that defined their brand, some reflective of the current brand and some aspirational. Words like *courageous*, *trusted*, *cinematic*, *thought-provoking* and even *badass* started to emerge. For me, these words started to become the beginning of visual design directions.

Our process was inspired by Brad Frost's [atomic design](http://bradfrost.com/blog/post/atomic-web-design/). But we used a simplified structure of templates made up of components, and components made up of individual styles. This structure influenced the visual design process and these components and styles would evolve into the final styleguide..

But first… typography. I don't know if the [web is 95% typography](https://ia.net/topics/the-web-is-all-about-typography-period) anymore (thanks to cat videos). But we still write a lot… and the reading experience was very important to get right for this redesign. FRONTLINE writes [longform](https://www.pbs.org/wgbh/frontline/article/the-battle-over-bunkerville/) and [shortform](https://www.pbs.org/wgbh/frontline/article/hhs-official-says-agency-lost-track-of-nearly-1500-unaccompanied-minors/) stories. The topics can be serious and challenging [something better here]. And the audience is increasingly comsuming stories on mobile devices. All of these factors dictated the process and decision making around article layout and typography. 

{% include inline-wide-split.html inline_img1='type_study_1.png' inline_img2='type_study_2.png'  class1='border' class2='border' alt1='' alt2='' %}

I experimented with typeface combinations in the browser so the team could experience them across devices. I looked at square sans serifs and monospaced fonts for meta information like bylines and dates. The display typeface for headlines allowed for the most experimentation: I looked at options from condensed and slightly casual (Cooper Hewitt? link) to a newsy slab (Adelle link). The article body typeface needed to work with the seriousness of the content. I wanted the letterforms to be more open for easier reading but also condensed to fit better on a smaller screen. I looked at (serifs like FF Tisa and …). 

I love the idea of style tiles (link) but I think the typical tile template is too small and limiting. I decided to choose a set of components that were representative of what this site would look like and create visual design directions out of those. Maybe they were more like element collages (Dan Mall link). I did all my visual design in HTML and CSS, it was a natural continuation of the wireframe prototyping process. 

Our team looked at these style directions with real fonts and styles rendered in the browser.

{% include inline-wide-split.html inline_img1='redesign_tile_1.jpg' inline_img2='redesign_tile_2.jpg' class1='border' class2='border' alt1='' alt2='' %}

{% include inline-wide-split.html inline_img1='redesign_tile_3.jpg' inline_img2='redesign_tile_4.jpg' class1='border' class2='border' alt1='' alt2='' %}

There were elements of all the style directions that the team resonded well to. We ultimately chose to iterate on the first direction which was the most elegant and minimal. 

For typefaces: [Cooper Hewitt](https://www.cooperhewitt.org/open-source-at-cooper-hewitt/cooper-hewitt-the-typeface-by-chester-jenkins/) was our choice for a display face. It looked great at large sizes and headlines looked serious but had personality. I chose [JAF Bernino](https://justanotherfoundry.com/bernini-sans) for body copy, and it was versatile enough to work for buttons and meta information text as well. It's condensed but still has clean and open forms that make reading easier. [make this better]

{% include inline-col-8.html class='border' inline_img='redesign_article.jpg' alt='' %}

[designing components, then checking them in comps]
[global nav and footer, thumbnail and slider component example from comps]

[components formed into final styleguide, made final development much easier]

{% include inline-wide.html inline_img='redesign_styleguide.jpg' alt='' %}

[film page with mobile example]

{% include inline-wide-split.html inline_img1='redesign_film.jpg' inline_img2='redesign_film_m.jpg' width='thin' class='mobile' class1='border' class2='border' alt1='' alt2='' %}

[investigation with mobile example]

{% include inline-wide-split.html inline_img1='redesign_investigation.jpg' inline_img2='redesign_investigation_m.jpg' width='thin' class='mobile' class1='border' class2='border' alt1='' alt2='' %}



