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

Back in January of 2023, I (Alex) finally finished my [VORON Legacy](/about/qcoral) by the [VORON Design](https://vorondesign.com/) team. No words could describe how awesome it felt to finally fulfill a dream I had so many years ago. I mean really, I had built a *massive* 3D printer from scratch! I immediately began hunting for my next challenge.

A few months prior, I had seen the [Positron](https://www.youtube.com/watch?v=X_QLxTVtyng) project by KRALYN Design. This design stuck out to for two reasons:

1. It fit inside a filament box, which was just the coolest thing ever
2. More importantly, it was filled with innovation, done entirely by one university student.

The second point was particularly meaningful to me though, since printers like the VORON Legacy I had just built were designed by entire teams of people. It made the task of designing a printer actually seem approachable.

With all that though, the Positron had one issue - it lacked accessibility. Not only did it cost upwards of $700+ USD, it also required custom CNC machined parts which I did not have access to. That's not to discount the project though - it's pretty remarkable overall. The project being inaccessible to me though, I decided to design my own instead; how hard could it really be? 

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

![neutrinomap](/images/neutrino/neutrinomaplr.png)

(You can download a high res version [here,](/images/neutrino/neutrinomaphr.png) complete with every detail)

Once I had this laid out, I began to actually work on what would become Neutrino.

<!-- ! Write chronologically!! -->


### Starting the development

<!-- Before 

- Challenges faced, what software to use, etc
- Krita
- Obsidian
- Paper sketches -->


### Working on each component

<!-- Being a portable printer, there were many design considerations I had to aim For -->

<!-- #### Template

- Prelude/context to the problem 
- Solution decided on and why 
- Problem(s) run into along the way 
- Possible final thoughts  -->

<!-- #### Innovations

Addtionally, I had just seen [this video](https://www.youtube.com/watch?v=bdCn-xrBLsE) by Thomas Sanladerer. In an attempt to minimize resonances, he fills a typical 3D printer with sand. While his results were rather disappointing, the idea intrigued me alot. This was because standard 3D prints use a type of infill called "gyroid" infill, which is technically a singular cavity.

- Sand? -->

#### Gantry Kinematics

Coming soon!

<!-- First thing to figure out was the kinematics setup. Being a portable printer, I needed something that was size-efficient and could print fast as well.

The most common setup are bed slingers. I ruled this out fairly early on for 2 reasons:

1. It was inefficient with size on the y-axis
2. The heavy bed would limit the speed, which was unacceptable since it needed to print fast.

(diagram here)

This narrowed my options down to 

Belts

Pulleys -->

#### Extrusion setup

Coming soon!

<!-- Extrusion was something I spent a lot of my time on.

Different options
- Sherpa mini
- Sharkfin
- Stealthburner
- Custom

The pros and cons -->

#### Z-axis

Coming soon!

<!-- Z-axis
- Heated bed
- Rubber thing -->

#### Electronics & Firmware

Coming soon!

<!-- Electronics

Modability

Firmware

- Custom PCB designs, the instructables tutorial

https://www.instructables.com/Small-and-Cheap-Tiny-OLED-for-Ender-3-stock-and-SK/

??? -->

#### PET Recycling unit

Being worked on!

### Final takeaways, next steps

<!-- - What it meant to me  -->