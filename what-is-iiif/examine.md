---
description: View objects in minute detail, share and cite with pinpoint accuracy
cover: ../.gitbook/assets/deepzoom.jpg
coverY: 55
---

# Examine

Tiled (or '[pyramid](https://training.iiif.io/iiif-online-workshop/day-two/fileformats.html)') images can be zoomed into at astonishing levels of detail, quickly and responsively, even if the image is very large. When a browser loads a tiled image, it doesn’t render every tile – just enough pixels to make the image legible. When a viewer starts to zoom in on a section of the image, more tiles are loaded - but only for that section - and this reduces the processing power needed to view the image in detail.

Take a look at [Rembrandt's Night Watch](https://hyper-resolution.org/view.html?pointer=0.329,0.001\&i=Rijksmuseum/SK-C-5/SK-C-5\_VIS\_20-um\_2019-12-21), from the Rijksmuseum, the largest and most detailed photo ever taken of a work of art. Strictly speaking, this is not a single digital image, but a composite of thousands of smaller images, as [the original painting was photographed in high resolution 8,439 times](https://www.rijksmuseum.nl/en/stories/operation-night-watch/story/ultra-high-resolution-image-of-the-night-watch). The sampling resolution is such that each digital pixel covers an area of the painting that is smaller than a red blood cell. This creates a composite image of 5.6TB - attempting to open a file that large would crash most browsers.

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption><p>Zoomed in detail from The Night Watch</p></figcaption></figure>

IIIF solves this problem - by tiling the object into digital fragments, viewers are able to zoom in, without lag, to see individual brushstrokes, hairline cracks, and particles of pigment.&#x20;

* Open the [Night Watch](https://hyper-resolution.org/view.html?pointer=0.329,0.001\&i=Rijksmuseum/SK-C-5/SK-C-5\_VIS\_20-um\_2019-12-21)
* Zoom in, and pan around - note that the coordinates in the address bar update as you move
* Try copying the address, and pasting it in a new tab - your location has been saved!

Being able to define and save a specific section of an image using its URL is significant. It means we can attach additional information to it through [annotation](annotate.md), enhancing the original. This might mean attaching a text transcript, overlaying another image for context or comparison, or adding a narrative commentary to support teaching and learning.
