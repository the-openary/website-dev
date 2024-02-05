---
title: "Development"
# meta title
meta_title: ""
# meta description
description: "A cheap, accessible printer that fits inside a spool box"
# save as draft
draft: false
---

{{< toc >}}

Note: Currrently, [Alex](/about/qcoral) is the only developer of the project, so this was written entirely by them, from their perspective.

### The <span class='pink-highlight'> Story </span>

Back in January of 2023, I (Alex) finally finished my [VORON Legacy](https://alexren.me/portfolio/voron) by the [VORON Design](https://vorondesign.com/) team. No words could describe how awesome it felt to finally fulfill a dream I had so many years ago. I mean really, I had built a *massive* 3D printer from scratch! I immediately began hunting for my next challenge.

A few months prior, I had seen the [Positron](https://positron3d.com/) project by KRALYN Design. 

{{< accordion "Positron Video" >}}

{{< youtube X_QLxTVtyng >}}

{{< /accordion >}}

This design stuck out to for two reasons:

1. It fit inside a filament box, which was just the coolest thing ever
2. More importantly, it was filled with innovation, done entirely by one university student.

The second point was particularly meaningful to me though, since printers like the VORON Legacy I had just built were designed by entire teams of people. It made the task of designing a printer actually seem approachable.

Costing upwards of 700+ USD and requiring custom CNC machined parts though, the project was unfortunately inaccessible to me. I decided to design my own instead; how hard could it really be?

Since my motivation to design a printer stemmed from accessibility issues, the that's what I decided to design Neutrino around. I sent out [surveys](https://tally.so/r/3xVgLE) to get an idea of issues that other people were facing. It didn't get enough responses for me to draw useful conclusions though. Instead, I decided to tackle almost every common issue I could think of with DIY 3D printers:

- **Cost** \
Most DIY 3D printer designs are just way too expensive in general. Sometimes they'll be labelled as "$200" and then have another $100 in shipping costs.
- **Custom parts** \
CNC machined parts or otherwise custom components are hard to obtain for many, so the design should omit them.
- **Complex build** \
I don't think someone should require an engineering degree to be able to put a good 3D printer together.
- **Plastic waste** \
3D printers use *a lot* of plastic, plastic which rarely gets recycled. I wanted to design my printer to be able to print with recycled plastic from water bottles. Much like the [Recreator 3D](http://recreator3d.com/)

I also wanted an answer to some "why not?" questions I've always had such as:

- **What happens if you buy the absolute cheapest parts?** \
3D printing communities tend to recommend certain sellers and manufacturers and to avoid the cheap parts like the plague, but I was always curious as to how bad it could really be. After all, they're still in business, right? (Spoiler alert: everything is pretty much the same)
- **What happens if you 3D print everything?** \
Almost every DIY 3D printer uses metal for the structural pieces, which makes up a large portion of the cost. I always wondered what would happen if you 3D printed them instead, even when much of the community recommended against it.

For the first few weeks, ideas to solve these problems lingered in my head, but nothing really came to fruition. During one particular dinner though, the vision for Neutrino came to me and I immediately sprinted upstairs. I spent the next 5 hours coming up with a flowchart:

<img src="/images/neutrino/neutrinomaplr.png" style="width: 80%">

(You can download a high res version [here,](/images/neutrino/neutrinomaphr.png) complete with every detail)

Once I had this laid out, I began to actually work on what would become Neutrino.

<!-- ! Write chronologically!! -->


### Getting started & Finding a workflow

Before I finished Neutrino, I never really designed anything more complicated than a weekend project; the design would span a couple weeks at most. As a result, I wasn't quite sure where to start with actually approaching the problem. I went through countless different software and methods to document ideas, learning a lot along the way.

Before then, I'd mostly just imagine the idea, make extremely rudimentary sketches, and then get to designing; that's pretty much how I started with this project. During this process, I swapped between a ton of different software, mainly for sketches.

{{< gallery dir="images/neutrino/getting-started-gallery" class="" height="400" width="400" webp="true" command="Fit" option="" zoomable="true" >}}

_Initially, I started with sketches made using [Excalidraw](https://excalidraw.com/)(Fig 1). For more technical drawings, I used [Krita](https://krita.org/en/) instead (Fig 2). I then figured that images and shapes would be easier to work with, instead of hand drawing every part (Fig 3). Later on though, I figured that it would be easier to just work out the dimensions in CAD software, so I used sketches to just represent concepts instead (Fig 4)._

For text-based notes and general planning though, I used [Obsidian](https://obsidian.md/) the entire time. I had learned about it through a friend a few months prior, and was already pretty familiar with it. It was useful for organizing my stuff into tasks

When it came to the software I'd actually use for designing, my choices were pretty straightforward. I had designed PCBs, made functional 3D printed parts, and programmed plenty of projects before. This was a matter of just combining them all. \
**In conclusion:**

- 3D modelling software: [**Fusion360**](https://www.autodesk.com/ca-en/products/fusion-360/personal)
- PCB Design software: [**KiCad**](https://www.kicad.org/)
- Programming: [**VSCode**](https://code.visualstudio.com/)
- Planning & Notes: [**Obsidian**](https://obsidian.md/)
- Sketches: [**Krita**](https://krita.org/en/)
- Version Control: [**Gitea**](https://about.gitea.com/)

<!-- Organizing the tasks into checklists -->

<!-- 
- Challenges faced, what software to use, etc
- Krita
- Obsidian
- Paper sketches -->


### The development itself

Being a portable printer, there were many design considerations I had to aim at. Each had their own specific problems to deal with. For ease of reading, I've blocked this section out into each respective component

<!-- #### Template

- Introduce constraints/prelude/context to the problem 
- Solution decided on and why 
- Problem(s) run into along the way 
- Possible final thoughts  -->

<!-- #### Innovations

Addtionally, I had just seen [this video](https://www.youtube.com/watch?v=bdCn-xrBLsE) by Thomas Sanladerer. In an attempt to minimize resonances, he fills a typical 3D printer with sand. While his results were rather disappointing, the idea intrigued me alot. This was because standard 3D prints use a type of infill called "gyroid" infill, which is technically a singular cavity.

- Sand? -->

#### Gantry Kinematics

Coming soon!

<!-- First thing to figure out was the kinematics setup. Being a portable printer, I needed something that was size-efficient and could print fast as well.

Before considering *any* setup though, I first set myself a constraint of being only allowed common 3D printing hardware, so I made a list of what I was allowed to use:

- MGN Linear rails
- Common stepper motors
- 

This does limit the amount of innovation that can be done, but I felt as though this would make the project much more approachable for adoption, which was one of the main goals of the printer.

Once that was out of the way, I was left with a couple options:

A core-XY style setup \
A bed slinger 

The most common setup are bed slingers. I ruled this out fairly early on for 2 reasons:

1. It was inefficient with size on the y-axis
2. The heavy bed would limit the speed, which was unacceptable since it needed to print fast.

(diagram here)

This narrowed my options down to  -->

#### Extrusion setup

Coming soon!

<!-- Constraints:

- Want to print PLA 
- Cheap
- Fast enough
- Accessible -->

<!-- Extrusion was something I spent a lot of my time on.

Different options
- Sherpa mini
- Sharkfin
- Stealthburner
- Custom

The pros and cons -->

#### Z-axis

Coming soon!

<!-- Constraints:

Wanted to print as many types of filament as possible, so a heated bed seemed like a good idea -->


<!-- Z-axis
- Heated bed
- Rubber thing -->

#### Frame & Base

Coming soon!

<!-- Sand, Z axis and rods... etc -->

#### Electronics & Firmware

Coming soon!

<!-- This mainly relied on the user experience
- Think ??

- Marlin -->


<!-- Electronics

Modability

Firmware

- Custom PCB designs, the instructables tutorial

https://www.instructables.com/Small-and-Cheap-Tiny-OLED-for-Ender-3-stock-and-SK/

??? -->

#### PET Recycling unit

Coming soon!

<!-- This was probably the most innovative part I tried.  -->

### Final takeaways, next steps

Coming soon!
<!-- 
The thing I want you to take away: when I started this project, I was, and still am, a regular person. I think it's easy to abstract away everything.  -->

<!-- - What it meant to me  -->