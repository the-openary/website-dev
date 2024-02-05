---
title: "Neutrino"
# meta title
meta_title: ""
# meta description
description: "A cheap, accessible printer that fits inside a spool box"
# save as draft
draft: false
layout: single
---

### What is Neutrino?

Neutrino is a 3D printer designed by [Alex.](/about/qcoral/) Wanting to make 3D printing more accessible, they designed Neutrino to be low-cost, portable, and easy to build. Currently, Neutrino is in alpha release and actively being worked on, with a proper YouTube video coming. In the meantime, you can find miscellaneous videos in the [discord.](https://discord.com/invite/VZFWGp7FHZ)

##### The files can be found here: https://github.com/the-openary/neutrino

{{< gallery dir="images/neutrino/gallery" class="" height="400" width="400" webp="true" command="Fit" option="" zoomable="true" >}}

In line with the ethos of The Openary, the development process of Neutrino is explained in-depth and accessible by anyone. It's *highly* recommended to check it out:

{{< button label="Learn about the development ➜" link="/neutrino/devinfo" style="solid" >}}

<!-- Useful information:
- Brief non-tech description of the project
- author (qcoral)
- status of the project 
- A brief story of how the printer was conceived; context basically
- Definitely story -->

### Features
<!-- 
- More technical information in general; keep it brief -->

Designed with accessibility mind, Neutrino attempts to resolve common 3D printing roadblocks. It can be built purely from off-the-shelf components and 3D printed parts, all for under $220 USD. No CNC machines or specialized equipment required.

##### Completed features:

- Fits inside a standard 200x200x70mm filament box
- Auto bed leveling
- Klipper firmware
- CoreXY kinematics
- Fully Open Source (MIT License)

##### Features currently in progress:
- **Self replicating capabilities** \
Neutrino aims to be [RepRap](https://reprap.org/wiki/RepRap) compatible, meaning that it can print all of its own parts. Unfortunately though, the base currently does not fit in Neutrino's build volume; this is actively being worked on.
- **PET Plastic bottle recycling** \
One of the most important issues in 3D printing is the plastic waste it generates. To solve this, an up-and-coming feature of Neutrino is to be able to recycle plastic bottles into filament, on the go. The [development page](/neutrino/devinfo) has more information on the status of this feature.

If this sounds like the printer for you, join the [discord](https://discord.com/invite/VZFWGp7FHZ) and get started!

{{< button label="Build your own ➜" link="/neutrino/building" style="solid" >}}

### How does it work?


![Neutrino Diagram](/images/neutrino/neutrinodiagram.png)
Once you're connected to the local WiFi network, you can upload 3D models through the web interface. The Raspberry Pi will process the 3D model's gcode, and then send it to the SKR Mini E3. The SKR Mini E3 then sends the signals to the rest of the printer to control it. _More coming soon, this is VERY WIP._

###### [Credits](/credits)
