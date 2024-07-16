+++
title = 'Gradient Map Filter'
date = 2024-07-15T10:20:48+08:00
draft = false
tags = ['react', 'javascript', 'html', 'css']
description = 'A web app for applying customizable gradient map filters to photos.'
summary = 'A web app for applying customizable gradient map filters to photos.'
+++

## Overview

I made a web app that lets users apply customizable filters to their photos using a gradient map, similar to the adjustment layer in Photoshop. You can try the app [here](https://gradient-map.netlify.app/) and check out the GitHub repo for this project [here](https://github.com/herenali/gradient-map-filter).

![A demo of the app](/images/projects/gradient-map/gradient-map-demo.jpeg)

## What is a gradient map?

A gradient map is used to map the colors in an image to the colors of a given gradient according to their brightness. Taking a black to white gradient as an example, the darker parts of the image are mapped to dark grey and black, while the lighter parts of the image are mapped to light grey and white. This turns your image into a greyscale image!

Numerous digital art programs have this functionality, including Photoshop, Clip Studio Paint and Procreate. Gradient maps are great for changing the mood and atmosphere of a photo. You can also use gradient maps to create cool duotone effects!

If you want to learn more about gradient maps, check out this [this guide](https://enviragallery.com/guide-to-gradient-maps-in-photoshop/)!

## Using the app

To upload your own image to apply a filter to, click on the "Choose file" button and pick an image.

The web app includes 4 default gradients which can be freely customized. **Switch between these 4 gradients by clicking on the gradient swatches at the top of the screen. To change a color in the gradient, click on the color swatch above the gradient bar and choose a new color using the color picker**. 

To add or remove a color from the gradient, click on the buttons "Add Color" or "Remove Color". Colors are added and removed starting from the rightmost color. Note that the minimum number of colors is 2.

If the filter feels to vibrant or sharp, you can tone down the effect by reducing the opacity of the gradient map. You can do so by adjusting the opacity slider above the "Add Color" and "Remove Color" buttons. **I personally recommend lowering the opacity to around 0.3 for a more natural effect**.

Once you're satisfied with the end result, click "Download Image" to download your new image!

## The implementation

> Persistence is key.

Stepping outside of your comfort zone is tough. To be honest, I wanted to give up multiple times while working on this project. I started out coding this project in Python with Django, but I ran into some issues on the way. After lots of failed troubleshooting, I decided to scrap my work and switch to Javascript. Fortunately, the logic for implementing the filter was mosly the same, so my earlier efforts weren't completely wasted. I also wanted to learn React, so I decided to choose it as my framework. Since this was my first time working with React, the React documentation was my best friend. React is also very popular, so lots of useful resources are available online. I still got stuck many times trying to get the filter to work, and nearly gave up when I couldn't get the filtered image to show up properly. At this point, I took a break from the project. As it turns out, taking breaks is one of the most important parts of work! After the break, I gave the project one last shot and things finally started working. Sometimes, not working can be more productive than working.

While working on the website, I also felt the importance of good design. Designers really *do* do tons of work to make apps and websites look good! I decided to settle with a minimalistic and responsive design, but there are still many, many parts I would improve about the design. Actually, my original design looked quite different. It looked fine on my laptop screen, but was unintuitive to work with on a mobile screen. In the end, I revamped the design and added extra CSS to ensure that the size of the gradient and the images were responsive. Responsive design is hard to get right, but looking back, it was completely worth the extra effort!

## Final thoughts

Surprisingly, trying to make this app user-friendly was harder than actually implementing the filter. Most people unfamiliar with photo-editing or digital art probably don't know what gradient maps are, so making my app as accessible and easy to understand as possible was a challenge. I'm really glad I didn't give up though - I think the end result is pretty cool!
