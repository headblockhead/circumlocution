Made by: @Edward Hesketh
Repository link: https://github.com/headblockhead/circumlocution/
Total hours so far: 3

- [x] I have a 3D printer or will be getting one before March 21st

# Circumlocution Journal

A documentation of the process of designing, modelling, and making my polar printer for [Hack Club's Infill YSWS](https://infill.hackclub.com/)/.

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
