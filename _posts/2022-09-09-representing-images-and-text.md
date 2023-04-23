---
title: Representing images and sound
author: Nikky Leone
date: 2022-08-09 20:55:00 +0000
categories: [Year 8, Computer Mathematics]
tags: [representing images and sound]
---

**Images also need to be converted into binary in order for a computer to process them so that they can be seen on our screen. Digital images are made up of pixels. Each pixel in an image is made up of binary numbers.**

**If we say that 1 is black (or on) and 0 is white (or off), then a simple black and white picture can be created using binary.**

**To create the picture, a grid can be set out and the squares coloured (1 – black and 0 – white). But before the grid can be created, the size of the grid needs be known. This data is called metadata and computers need metadata to know the size of an image.** If the metadata for the image to be created is 10x10, this means the picture will be 10 pixels across and 10 pixels down.

This example shows an image created in this way:

<img src="https://bam.files.bbci.co.uk/bam/live/content/zdcxfg8/large" alt="graph"> 
 

# Adding colour

**The system described so far is fine for black and white images, but most images need to use colours as well. Instead of using just 0 and 1, using four possible numbers will allow an image to use four colours.** In binary this can be represented using two bits per pixel:

- 00 – white
- 01 – blue
- 10 – green
- 11 – red

While this is still not a very large range of colours, adding another binary digit will double the number of colours that are available:

- 1 bit per pixel (0 or 1): two possible colours
- 2 bits per pixel (00 to 11): four possible colours
- 3 bits per pixel (000 to 111): eight possible colours
- 4 bits per pixel (0000 – 1111): 16 possible colours
…
- 16 bits per pixel (0000 0000 0000 0000 – 1111 1111 1111 1111): over 65 000 possible colours

**The number of bits used to store each pixel is called the colour depth. Images with more colours need more pixels to store each available colour. This means that images that use lots of colours are stored in larger files.**

# Image quality

**Image quality is affected by the resolution of the image. The resolution of an image is a way of describing how tightly packed the pixels are.**

**In a low-resolution image, the pixels are larger so fewer are needed to fill the space. This results in images that look blocky or pixelated. An image with a high resolution has more pixels, so it looks a lot better when you zoom in or stretch it. The downside of having more pixels is that the file size will be bigger.**

# Representing sound

**Sound needs to be converted into binary for computers to be able to process it. To do this, sound is captured - usually by a microphone - and then converted into a digital signal.**

**An analogue to digital converter will sample a sound wave at regular time intervals. For example, a sound wave like this can be sampled at each time sample point:**

<img src="https://bam.files.bbci.co.uk/bam/live/content/zqg72hv/large" alt="graph"> 

The samples can then be converted to binary. They will be recorded to the nearest whole number.

sampling does not take into account what the sound wave is doing in between each time sample.

**When sampling an analogue waveform, the resulting digital sound wave is not exactly like the original.
This means that the sound loses quality as data has been lost between the time samples. The way to increase the quality and store the sound at a quality closer to the original, is to have more time samples that are closer together.** This way, more detail about the sound can be collected, so when it’s converted to digital and back to analogue again it does not lose as much quality.

**The frequency at which samples are taken is called the sample rate, and is measured in** [**Hertz (Hz)**](https://en.wikipedia.org/wiki/Hertz). 1 Hz is one sample per second. **Most CD-quality audio is sampled at 44,100 or 48,000 KHz.**


