Made by: @Edward Hesketh
Repository link: https://github.com/headblockhead/circumlocution/
Total hours so far: 10

- [x] I have a 3D printer or will be getting one before March 21st

# Circumlocution Journal

A documentation of the process of designing, modelling, and making my polar printer for [Hack Club's Infill YSWS](https://infill.hackclub.com/).

## Hour 1

<sup>began on UNIX Timestamp 1739815200</sup>

## Design sketch 

I started drawing up a design sketch for what my printer could look like using GIMP, and came up with a design I was happy with.
(15 mins)

![A4 first-draft design drawings](https://cdn.hack.pet/slackcdn/d91bc4b31b23c046a705fee6ea968fa4.png)

Then, I started planning out the rough mechanical design for how the printer's motors would be positioned.
(20 mins)

![A4 hand-drawn rough mechanical design](https://cdn.hackclubber.dev/slackcdn/0cba194f1f4cf945c3f0f4cda7f216af.png)

I took a few measurements from the ender 3, and did a little research, and decided on 2020 aluminium extrusion to use for the frame, and M10 threaded rod for the Z-axis. I have a feeling that these decisions might change later, but for now, that's what I'll use for the CAD models. I'm thinking of using FreeCAD for the printer, but I'm pretty sure I'll regret it 😆! I also researched the time+date of the Rocky Mountain RepRap Festival to ensure I could actually make it there, without missing too much schoolwork or any exams that I'd have to do tons of catch-up for. Hopefully, if I make it, my school will allow me to take a day or two off to attend.
(25 mins)

## Hour 2

<sup>began on UNIX Timestamp 1739819370</sup>

I started modelling the 2020 extrusion in FreeCAD for use in my design based on this reference diagram from [www.tnutz.com](https://www.tnutz.com/product/exm-2020/).

![The reference image for the 2020 extrusion](https://cdn.hackclubber.dev/slackcdn/7771bdcac71cdee5df4468b976001336.png)

This is the end result:

![FreeCAD Sketch showing the 2020 extrusion's cross-section](https://cdn.hackclubber.dev/slackcdn/1f70b50b7acbe0344b657bcd1724ec4a.png)
![FreeCAD screenshot showing the extrusion, extruded](https://cdn.hack.pet/slackcdn/8ca8864171033d78c575cc6f35eb8825.png)

(60 mins)

## Hour 3

<sup>began on UNIX Timestamp 1739885638</sup>

I started modelling the Z axis. I looked at the design of the Ender 3 for an example of how a Z-axis could be assembled:

![Ender 3 Z-Axis picture](https://cdn.hackclubber.dev/slackcdn/60de35011490539cf4fd5e0239219243.png)

And I moddled some 2040 extrusion.

![2040 extrusion model](https://cdn.hackclubber.dev/slackcdn/94690d0a2c914efde01b9fe4447c6ce6.png)

I also sourced [a model for a NEMA 17 stepper motor](https://www.thingiverse.com/thing:6761583/files), to use as reference for the 3D printed parts.

![NEMA 17 stepper screenshot](https://cdn.hackclubber.dev/slackcdn/40f02e0b98249b96c1ccbab54d68d6bd.png)

Finally, I generated a model for the threaded rod - a TR8x8 lead screw (30cm).

![Lead screw model](https://cdn.hackclubber.dev/slackcdn/6c7c4cf13d735035023bc473e769a3a6.png)

## Hour 4

<sup>began on UNIX Timestamp 1739889914</sup>

I found [an existing NEMA 17 motor mounting bracket](https://www.123-3d.co.uk/123-3D-Metal-mounting-bracket-for-NEMA17-stepper-motor-90-L-bracket-i2129-t14804.html) made of sheet metal, and modelled it to see if it could fit the 2040 extrusion. I spent 50 minutes creating the model, but it isn't compatible with the 2040 rails, it just looks like it *could* be. Oh well! Looks like I'll have to design a part for this bit. At least I have accurate dimensions though!

![NEMA 17 motor mount](https://cdn.hackclubber.dev/slackcdn/05b30cda79c101e34b259e96be0f15b3.png)

I've had no regrets using FreeCAD so far, the 1.0.0 version improved a **lot** since ~0.2. Fusion 360 would be *way easier*, but it's not exactly in the 'open source spirit' in my opinion, because if Fusion dies, the project dies too. But FreeCAD's code will (hopefully) be available for free, and for forever. 

I'm keeping the right angle bracket model around just in case I am able to use it somewhere else, I'm getting my time's worth out of that model someday!

I also found [some brackets](https://www.123-3d.co.uk/123-3D-Blind-corner-connector-for-aluminium-2020-profile-123-3D-brand-i1590-t14575.html) for attaching the extrusions together, could be worth a look at next hour.

## Hour 5

<sup>began on UNIX Timestamp 1739893575</sup>

I modelled the 5-8mm shaft coupling part:

![coupling part](https://cdn.hackclubber.dev/slackcdn/1c53eb03b7c93efc7df3e740816198a9.png)

And created the first 3D-printable part, the mounting bracket for the motor.

![motor mounting bracket](https://cdn.hack.pet/slackcdn/cd3028f52420394428f062ef7cd5f573.png)

## Hour 6

<sup>began on UNIX Timestamp 1739897976</sup>

I have found the correct sizes of fasteners (nuts/bolts/TSlots) for the rails and motors that I am using, and have added them to the CAD model, in roughly the correct places, to ensure that my parts don't overlap the heads of any of the screws I will need to install.

![motor and extrusions with screws and slots](https://cdn.hack.pet/slackcdn/9ab6941896ad23120a4126bccc9aa6e2.png)

Finally, I renamed all of the parts to have (mostly) sensible names:

![parts list with sensible names](https://cdn.hackclubber.dev/slackcdn/c091daf3599890aa7fd94361db321e48.png)

## Hours 7-9

<sup>hour 7 began on approx. UNIX Timestamp 1740168000 and 8-9 on approx. UNIX Timestamp 1740256200</sup>

I have made quite a lot of undocumented progress on-and-off through short sessions in my free time, so in summary the changes are:
- Added a trapezoidal nut to follow the lead screw
- Switched to using hex bolts instead of phillips screws
- Set the position of objects manually, to avoid imprecision from visual only alignment
- [Found a pulley](https://www.123-3d.co.uk/123-3D-GT2-high-resolution-timing-belt-pulley-20-teeth-6mm-belt-5mm-bore-GT2-20T-W6-B5-i2081-t14815.html) for the X axis belt, [and a similar-enough model](https://grabcad.com/library/gt2-pulley-20-tooth-id-6mm-1)
- Built a carriage to follow the nut by holding the nut using screws screwing into heat-set inserts

![a screenshot of the whole assembly with changes as described above](https://cloud-d1we5mzy3-hack-club-bot.vercel.app/0image.png)

## Hour 10

<sup>began on UNIX Timestamp 1740416875</sup>

I planned out the position for the rollers to follow the Z axis:

![](https://cloud-cyfuz2z3i-hack-club-bot.vercel.app/0image.png)

Added the rollers, and started re-building the carriage.

![](https://cloud-aa22v5w8t-hack-club-bot.vercel.app/0image.png)
