---
layout: page
title: "KeyPoard Build Log"
date: 2012-08-11 05:39
comments: true
sharing: true
footer: true
---
I got the case from the machine shop!
![Case](/images/keypoard/keypoard-al-case.jpg)

I choose a slightly different key switch hole to make it more machinable, but allowed the switch tops to be replaceable without desoldering.
![Case](/images/keypoard/keypoard-al-case-zoom.jpg)

Here it is with the Cherry MX Blues.  The fit is so tight!  There is very little wiggle of the switches even without a pcb.  The power of precision CNC machining.
![Case](/images/keypoard/keypoard-switches.jpg)

And with R3 only blank key caps!
![Case](/images/keypoard/keypoard-keycaps.jpg)

I choose R3 only key caps so the entire keyboard would be flat.
![Case](/images/keypoard/keypoard-flat.jpg)

Hand wired the matrix.
![Case](/images/keypoard/keypoard-matrix.jpg)

The trackpad fits perfectly and clicks without friction!  But I did screw up the corner radius so there is a gap.  Stupid imperial vs metric strikes again!
![Case](/images/keypoard/keypoard-trackpad.jpg)

The radius in the back matches the trackpad perfectly!  But there is a gap in order to make it machinable.
![Case](/images/keypoard/keypoard-trackpad-back.jpg)

Like lowploy, I wired the rows and cols with ribbon cable.
![Case](/images/keypoard/keypoard-controller-wiring.jpg)

Wired the ribbon cables to the controller.  You can tell I am pro at soldering!
![Case](/images/keypoard/keypoard-controller.jpg)

For the firmware, I first tried to use Hasu's, but I wired the matrix backwards to what the code expects.  I attempted to flip the matrix in the code, but it didn't work and I couldn't figure it out.

So I gave up and tried the Phantom firmware because it was quite a bit more simpler.  The code already expects reading from the rows, so all I had to do was reconfigure the code.  Unfortunately the code hardcoded which pins are row/cols so I had to generalize that.

I fired up the code and only found 2 mistakes in the physical matrix and had to resolder the the ribbon cable to the controller to clean up the stray wires.

Otherwise everything just mostly worked!  I actually can't believe how little debugging I had to do (ignoring the fact I couldn't get my modified version of Hasu's code to work).

