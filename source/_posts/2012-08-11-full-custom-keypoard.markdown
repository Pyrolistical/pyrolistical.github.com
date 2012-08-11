---
layout: post
title: "Full Custom KeyPoard"
date: 2012-08-11 04:47
comments: true
categories: [keyboard, hardware, custom]
---

![KeyPoard](/images/keypoard/keypoard-finished.jpg)

####Feature Summary:
 - single piece machined aluminum case
 - flat split true matrix layout
 - large hand separation
 - ten keyless
 - Macintosh layout with symmetric standard modifiers
 - integrated Apple Magic Trackpad and palm rest
 - Cherry MX Blue keyswitches
 - full n-key rollover matrix

Ancestry of KeyPoard is a cross between HumbleHacker and Apple Wireless Keyboard.

### Motivation

I've been looking for the perfect keyboard and was disappointed when I did not find it.

I own a Kinesis Contoured and its where I fell in love with the non staggered layout, but I really didn't like some of the layout choices such as putting the +/= on the top left.  Sure I could remap it, but there isn't enough room to put it in the right place.  So I knew I wanted a keyboard with a more standard layout.  Which means [TypeMatrix](http://typematrix.com/) and [HumbleHacker](http://www.humblehacker.com/keyboard/) were also out.

The other keyboard I regularly use is the Apple Wireless Keyboard.  I really like the design philosophy of Apple products where everything is beautifully designed yet functional.  This lead me to design a keyboard as simple as possible with the fewest parts.

Keyboards have so much legacy behind them. Modern keyboards copy the staggering of keys mindlessly from the original typewriters.  Apple showed us a completely flat keyboard works, which is unlike most keyboards with varying row heights.

I wasn't going to find my perfect keyboard.  I was going to have to make it myself which is where the story of KeyPoard begins.  I'll let you figure out why the b is upside down.

###Layout

![Layout](/images/keypoard/keypoard-layout.png)

This layout emulates the standard Macintosh, except I had room to sneak in another control key.  This makes the modifers nice and symmetric.

The keyboard uses R3 keycaps to make the entire keyboard flat like the Apple Wireless Keyboard.  The keywells have good hand separation accomplished with an integrated Apple Magic Trackpad in the middle.

###Case

![Case](/images/keypoard/keypoard-case.png)

The case is machined out of a single block of aluminum.  Yes this makes it expensive, but this is what you need to do for simplicy of design.

The integrated palm rest is to reduce wrist angle.  Regular keyboards are terrible for the wrist with their positive keyboard slopes.  The keys are as low as possible without the need to reach deep into the keywells to further minimize wrist angle.

###Electronics

I am not creating a PCB for this keyboard.  Instead I took inspiration from lowpoly and going to hand wire the matrix like he did with [The Apple M0110 Today](http://deskthority.net/workshop-f7/the-apple-m0110-today-t1067.html).  As for the controller I will be using a [Teensy 2.0](http://www.pjrc.com/teensy/index.html).

###Firmware

I was originally going to use hasu's [tmk_keyboard](https://github.com/tmk/tmk_keyboard) firmware, but in the end I used the Phantom-Keyboard firmware which has now been moved to [Teensy-Keyboard](https://github.com/BathroomEpiphanies/Teensy-Keyboard).  The history is a bit lost now, but the current Teensy-Keyboard firmware integrated my [configuration enhancements](https://github.com/Pyrolistical/Phantom-Keyboard/commit/4b349e51e3681839322333da7651bd6f1cbfdea1).

###Result

I've been using the KeyPoard for the last few days and its amazing!  Since I was used to the Kinesis Advantage matrix layout I was able to go at full typing speeds with relative ease.  There were a few minor build hickups and for all the details see the [Build Log](keypoard-build-log).

Note: This was originally posted on geekhack.org, but due to their ups and downs I've decided to permanately move this post here.

