---
layout: page
title: Software Development
permalink: /software/
---

Overview and status updates on software developed to support open source course design and creation. See [tools](/tools/) for external tools and resources.

### gist
The goal of this project is to experiment with video content creation more akin to software development. If an image needs to be swapped for copyright infingement, or a new narrator recorded audio for the video, the content could be swapped out and the updated video exported without having to ever open a cumbersome video editing program. One major difference is that with the inclusion of a simple ui video creation would be very simple and "text forward". Audio files in video editing just display waveforms, which is helpful only after you've tracked down the word. After running an audio recording through speech to text software, precise time-stamps could be generated and used as a 'transport' insted of a typical timeline.

#### Project goals
- compose a module video without using a mouse or gui
- export videos with a single command after swapping assets
- batch export entire course
- "text forward" asset syncing to transcripted audio
- create stylistically symetrical content
- free up more time for creating great animations/assets
- create organized structure for asset searching/sharing between projects
- easy to port to web app or remote instance

#### tools/libraries used
- python backend 
- melt framework video compiling w/ python bindings
- flask/webenv ui (javascript)

### Example UI
![UI 1](/images/text-forward-ui)
#### a "text forward" interface
This first window one would be able to select an asset, giving it a unique color identifier. The script window would be linked to a json file with the time-stamps of words so that highlighting sections would create start and end points for the assets. Each tab would contain a different layer: animations, slides, background.

![UI 2](/images/text-forward-ui-2)
#### basic page arrange macros
In this second window each layer could be arranged to set max dimensions and offsets. Dimentions would be click + dragable, but fixed fractional dimensions could be clickable for strict proportions. The assets would then be resized by their limiting dimenstion (height or width) so that they do not exceed the boundaries.