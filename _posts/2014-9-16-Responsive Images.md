---
layout:post
title: Responsive Images
---

##What's the Deal with Responsive Images

Responsive images have many uses from making sure that users are seeing the appropriate image based on their browser and screen.
There is also the issue of load time and effiency of a site which can be aided by having the correct image responses come into play.
Something that has been a problem in the past with responsive images is the lack of uniform consensus on how to really deal with this.
One of the culprits was lack of compliance with the browser end of things for a while but the W3C has started to get its act together.
As of now there are a lot of new ways to get around these problems using things like the picture tag as seen in the code below.
There are also one stop solutions like Picturefill 2.0 that use some of the existing tags to make life easier.  All this is just a brief overview
there are still some of the old hacks that may be appropriate in certain instances like using javascript, background image swaps in media quieries(see below), or even the old percentages on width.

I can see why this is such a debated topic because for the longest time you really didn't have to deal with much other than desktop design.
With the dawn of mobile phone browsing, tablets, phablets, retina displays, 4k now and everything inbetween.  This really left a lot of 
websites back in the stoneage and struggling to adjust their sites for modern times.  The question people with site like that have to adk themselves
are numerous and you can see why this would be very frustrating.

##This is what the Picturefill would look like

```
<picture>
  <source media="(min-width: 600px)" srcset="large-1.jpg, large-2.jpg 2x">
  <img alt="A fat dog" src="small-1.jpg">
</picture> 
```
##This is what the CSS media queries look like

```
( (min-device-pixel-ratio: 1.5) and (min-width: 20.001em) and (max-width: 35.999em) ) or
( (max-device-pixel-ratio: 1.5) and (min-width: 120.001em) ) or
( (min-device-pixel-ratio: 1.5) and (min-width: 60.001em) )
```
