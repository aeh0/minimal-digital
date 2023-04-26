---
description: View objects in minute detail, share and cite with pinpoint accuracy
cover: ../.gitbook/assets/deepzoom.jpg
coverY: 55
---

# Examine

Tiled (or '[pyramid](https://training.iiif.io/iiif-online-workshop/day-two/fileformats.html)') images can be zoomed into at astonishing levels of detail, quickly and responsively, even if the image is very large. When the browser loads a tiled image, it doesn’t show every tile – just enough to make the image legible. If you start to zoom in on a smaller section, more tiles will be loaded, but only for that section, and this reduces the processing power needed to view the image.

Take a look at [Rembrandt's Night Watch](https://hyper-resolution.org/view.html?pointer=0.329,0.001\&i=Rijksmuseum/SK-C-5/SK-C-5\_VIS\_20-um\_2019-12-21), from the Rijksmuseum, the largest and most detailed photo ever taken of a work of art. What you are viewing is a digital composite of thousands of smaller images, as [the original painting was photographed in high resolution 8,439 times](https://www.rijksmuseum.nl/en/stories/operation-night-watch/story/ultra-high-resolution-image-of-the-night-watch). The sampling resolution is such that each digital pixel covers an area of the painting that is smaller than a red blood cell. This created a composite image of 5.6TB - large enough to crash most browsers.

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

IIIF solves this problem - by tiling the object into digital fragments, viewers are able to zoom in, without lag, to see individual brushstrokes, hairline cracks, and particles of pigment.&#x20;

* Open the [Night Watch](https://hyper-resolution.org/view.html?pointer=0.329,0.001\&i=Rijksmuseum/SK-C-5/SK-C-5\_VIS\_20-um\_2019-12-21)
* Zoom in, and pan around - the coordinates in the address bar update as you move
* Try copying the address, and pasting it in a new tab - your location has been saved!

Being able to define and save a specific section of an image using a URL, means we can attach additional information to it through [annotation](annotate.md), enhancing the original. This might mean attaching a text transcript, overlaying another image for context or comparison, or adding a narrative commentary to support teaching and learning.
