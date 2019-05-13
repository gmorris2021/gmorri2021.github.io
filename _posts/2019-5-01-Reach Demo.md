---
layout: post
title: Week 5 and Reach Demo!
---

Welcome back again everyone! It has been a long week with almost no sleep, but we finished!

This week, in moving from our baseline to reach demos, we had three main things that we worked on. Revamping our pressure sensors, moving to multichamber inflation, and cleaning up our product. In terms of new parts needed this week, we needed:

1. Copper foil for our pressure sensors
2. Smaller pillows for our multichamber pillow
3. 3D printed parts to split the tubing from the blower
4. A new air compressor that was larger and more powerful.

For the first goal, we realized that needed to use the sheets flat instead of folded, and that we needed to find a way to attach wires (not banana clips) in order to cover more surface area and make the pillow actually useable. We realized, that using copper foil alongside the pressure sheets, we could accomplish both. We first made a small prototype before we created the larger one for our pillow. What we did was we layered two sheets with three rows each of copper foil, put these rows perpendicular, and then put a pressure sheet inbetween them. Next, we soldered wire to the ends of the copper foil and hooked up 3 ends to power, 3 to the analog out, and 3 to ground. The power end and ground end were opposite one another, with the analog end perpendicular to them. This can be seen below:

![_config.yml]({{ site.baseurl }}/images/Reach1.png)

Once this was all done, we hooked this up to the mbed in order to measure pressure. This was done as follows. The pressure sheets layed on top of one other create a voltage divider for each power column, so what we did was send power to one of the columns, measure the analog out at the three outputs (one for each row), we then sent power down the next column, repeated the process, and finally sent it down the last column and repeated the process. In doing so, using the fact that these were voltage dividers, we were able to traingulate the position of the pressure using math based on the analog values out. Once we got the prototype working, we moved on to a much bigger grid, that can be seen below.

![_config.yml]({{ site.baseurl }}/images/Reach2.png)

This grid had four rows and four columns, in order to be more accurate in determining the position on the pillow, as well as be larger in order to cover more space. With this done, we moved onto working on integrating the smaller pillows. This was done through using solenoids and the smaller pillows alongside our 3D printed parts. These can be seen below:

![_config.yml]({{ site.baseurl }}/images/Reach4.png)

These parts were created in order to put one tube in with air and two tubes out carrying the air. Meanwhile, for the actual pillow we put together four smaller pillows, alongside tubes into the four pillows. This can be seen below:

![_config.yml]({{ site.baseurl }}/images/Reach3.png)

Once this was done
