---
title: "Neutrino"
# meta title
meta_title: ""
# meta description
description: "A cheap, accessible printer that fits inside a spool box"
# save as draft
draft: false
---

#### Overview

A 3D printer designed to be cheap, accessible, and portable. 

{{< accordion "YouTube video" >}}

Coming soon!

<!-- {{< youtube ResipmZmpDU >}} -->

{{< /accordion >}}

---

#### Features
- Fits in a 200x200x70mm volume
- Under $300 CAD (using the attached BOM)
- Uses common, off-the-shelf parts
- Completely self replicating* (currently the base is not printable on itself)

*planned

---

#### Getting started

**The repository and all the files for the printer can be found here: https://github.com/the-openary/neutrino**

- The Bill of Materials (BOM) is currently missing screw counts, that will be added soon.
- STLs are not yet exported, you will have to manually open the CAD file and export them. I recommend using [Fusion 360](https://www.autodesk.com/ca-en/products/fusion-360/personal) 
- Assembly guides, explanations, and documentation coming soon! Join the discord for help in the meantime.

---

#### FAQ

**Can I see a video?**\
There are short clips that can be found in the discord. Currently working on a proper release video, will try and get that out soon<sup>tm</sup>.

**Where's the extruder?**\
Great question! The Neutrino is designed to use a Sherpa Mini in bowden configuration. Due to copyright, it cannot be included in the CAD. It can be found [here](https://github.com/Annex-Engineering/Sherpa_Mini-Extruder). Totally awesome design.

**Why a Bowden Setup?**\
Initially the printer had a Direct Drive setup, but this was later swapped to Bowden. There were a couple reasons for this
- Faster printing
- Short tube length
- Easier maintenance
- Easier to explain to others
    - Being a portable printer, many people who have never seen a 3D printer see it. I think this makes Neutrino double as an educational/inspirational tool and for that reason it is easier to explain the separate parts of a Bowden extruder vs a DD setup. 

**Where can I source my parts?**\
Anywhere you can find them. The `BOM.xlsx` file contains links to all the sources that I used during development. The printer itself uses all standard 8mm + M3 hardware. Use AliExpress, Amazon, spare parts, etc. Unfortunately you will need to print your own parts for now, but that will change soon.

**Is there an assembly guide?**\
Not yet, working on that soon. For now you should just use the CAD. There is also the [discord](https://discord.gg/VZFWGp7FHZ) for help. I can assist you personally there.

**Why the name "Neutrino"?**\
The [Positron](https://github.com/KRALYN/PositronV3) project was a huge inspiration for me whilst designing this project. Seeing the innovation process and Kralyn's willingness to tackle problems was a huge motivator for me. While Neutrino was originally a codename, I believe it fits pretty well. 

---

{{< accordion "TODO:" >}}

- [ ] Make the base self replicating
- [ ] Misc clearance fixes
- [ ] Add pin breakout connector
- [ ] Add PET Recycling integration

{{< /accordion >}}

#### [Credits](/credits)