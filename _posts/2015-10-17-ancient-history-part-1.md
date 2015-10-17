---
layout: post
title: "Sapphire's Ancient History, Part 1: the stuff you can see"
author: xunker
modified:
excerpt: "Showing the history of Sapphire, from the first version until now."
tags: []
comments: true
---
Before Sapphire really existed, there was just the idea: can you make a Bluetooth remote-control fit inside the hands of a crutch? At the time I didn’t know a thing about micro-controllers, electronics or 3D printing but I still needed to create a proof of concept device.

Using a handful of off-the-shelf hardware, a soldering iron and some hand tools, the proof of concept was built in a month of weekends.

[![Components on breadboard]({{ site.url }}/images/ancient_history/IMG_0720_small.jpg)]({{ site.url }}/images/ancient_history/IMG_0720.jpg)
{: .image-pull-right}

The main hardware is the [Adafruit Bluefruit EZ-Key](https://www.adafruit.com/products/1535) (black breadboard), which is basically a very small Bluetooth keyboard. When you send a signal to one if its 12 I/O lines, it sends a keystroke to whatever computer it is paired with. The buttons (green breadboard) give those signals. The [Arduino Micro](https://www.arduino.cc/en/Main/ArduinoBoardMicro) on the yellow breadboard is just there to act as a power supply.

[![Components on breadboard with battery]({{ site.url }}/images/ancient_history/IMG_0721_small.jpg)]({{ site.url }}/images/ancient_history/IMG_0721.jpg)
{: .image-pull-left}

Of course, having a whole Arduino Micro just to get power was pretty wasteful and it was eventually swapped with a bunch of AAA batteries. The project was finally, truly wireless.

After I proved it could work on batteries, I had to make a way to mount it to the crutch and have buttons. This was done by drilling holes in the existing handle "plug" that came with the crutch and using plastic that can be molded in hot water to hold the switches. Putting it all together you get something it pretty close to the Sapphire of today.

[![First sapphire proof-of-concept]({{ site.url }}/images/ancient_history/IMG_0729_small.jpg)]({{ site.url }}/images/ancient_history/IMG_0729.jpg)
[![First sapphire proof-of-concept]({{ site.url }}/images/ancient_history/IMG_0725_small.jpg)]({{ site.url }}/images/ancient_history/IMG_0725.jpg)
{: .image-pull-left}

Rocking the middle switch will change the track and pushing it in will toggle "play" or "pause". The buttons to the left and right are volume control and the final button at the top is the "Home" button on iOS and Android. Even though the design wasn't really ergonomic (and *was* pretty ugly), it proved that is could be built. This was July of 2014.

I then built over a dozen test controllers out of foam modeling clay; no wiring or electronics, just tests to find the right size and the best place for the switches.

[![Test controller made of clay foam]({{ site.url }}/images/ancient_history/IMG_0760_small.jpg)]({{ site.url }}/images/ancient_history/IMG_0760.jpg)
[![Test controller made of clay foam]({{ site.url }}/images/ancient_history/IMG_0764_small.jpg)]({{ site.url }}/images/ancient_history/IMG_0764.jpg)
[![Test controller made of clay foam]({{ site.url }}/images/ancient_history/IMG_0767_small.jpg)]({{ site.url }}/images/ancient_history/IMG_0767.jpg)
[![Test controller made of clay foam]({{ site.url }}/images/ancient_history/IMG_0772_small.jpg)]({{ site.url }}/images/ancient_history/IMG_0772.jpg)
{: .image-center}

After I found a design I thought would work, I needed to make it out of stronger stuff so I could wire it up and actually use it. I ended up using regular modeling clay formed into a semi-circle (using a light- bulb as the mold!) and then used a knife and a hobby drill to make the spaces for switches and wires. After baking the clay, soldering the components and mounting them, it was ready to be used for the first time.

[![First version made from red modeling clay]({{ site.url }}/images/ancient_history/IMG_0866_small.jpg)]({{ site.url }}/images/ancient_history/IMG_0866.jpg)
{: .image-pull-right}

This was a good way to test the fitting and get things wired but the clay was brittle and ended up cracking the first time I used it. To make a stronger version I made a mold using part of a soda can some casting material from a craft store.

[![Making mold of first version]({{ site.url }}/images/ancient_history/IMG_0872_small.jpg)]({{ site.url }}/images/ancient_history/IMG_0872.jpg)
[![Making mold of first version]({{ site.url }}/images/ancient_history/IMG_0874_small.jpg)]({{ site.url }}/images/ancient_history/IMG_0874.jpg)
{: .image-pull-left}

I put the switchgear in to the mold, soldered it up and then poured liquid JB-Weld over it.

[![Pouring JB-Weld in to mold]({{ site.url }}/images/ancient_history/IMG_0877_small.jpg)]({{ site.url }}/images/ancient_history/IMG_0877.jpg)
[![Second version, made from cast JB-Weld]({{ site.url }}/images/ancient_history/IMG_1031_small.jpg)]({{ site.url }}/images/ancient_history/IMG_1031.jpg)
{: .image-pull-left}

The result was a very tough, but very bad-smelling, copy. It also took a lot of time to wire up and cast, and the switches couldn’t be replaced without scrapping the whole unit so I knew this would’t do for long.

I used this version for about 4 months until I bought a 3D printer and was able design a printable and repeatable assembly.

With a 3D printer, time to assemble the control hardware has gone from about 4 hours to under 1 hour. It can also be disassembled and parts inside can be replaced without having to snap the whole module.

[![Pile of 3D printed test parts]({{ site.url }}/images/ancient_history/IMG_1110_small.jpg)]({{ site.url }}/images/ancient_history/IMG_1110.jpg)
[![Evolution of the 3D printed control module]({{ site.url }}/images/ancient_history/IMG_1108_small.jpg)]({{ site.url }}/images/ancient_history/IMG_1108.jpg)
[![Current 3D printed control module]({{ site.url }}/images/ancient_history/IMG_1075_small.jpg)]({{ site.url }}/images/ancient_history/IMG_1075.jpg)
{: .image-center}

The production versions will probably move to injection-molded plastic, but with the advancements made in 3D printing it may make more sense to continue to use 3D printed hardware.