---
description: Analyse digital objects from different institutions side-by-side
---

# Compare

There may be times when you want to compare multiple digital objects from repositories, that might be on different sides of the world. Preliminary sketches with a final artwork, or multiple versions of a manuscript. IIIF supports this too, using Mirador a web-based viewer

### Using the Mirador viewer

* Find a IIIF manifest: A manifest is a JSON file - a unique link combining the digital images you want to view, and their metadata. See this guide to [finding IIIF images](finding-iiif-images.md) for more information about manifests, and how to find them in digital collections or repositories that support IIIF, such as the [British Library](https://iiif.io/guides/guides/bl.uk/), [Harvard](https://iiif.io/guides/guides/library.harvard.edu/), [Library of Congress](https://iiif.io/guides/guides/loc.gov/), or the [Bodleian](https://iiif.io/guides/guides/digital.bodleian.ox.ac.uk/).
* Once you've found a IIIF manifest, [open the Mirador viewer in your web browser](https://projectmirador.org/demo/). This will open Mirador with a default set of images. Use the X button in the top right of each to clear the default images.
* To load a IIIF manifest into Mirador, click on the '+ Start here' button in the top left corner of the viewer. You'll see a list of sample manifests - click 'Add resource' in the bottom right to add a new one. Paste the URL of a IIIF manifest into the text field and click 'Add'. Click on the new row to load the images into the viewer, and display them in the main window. Here are some manifests (JSON links) of three different 15th century manuscripts of Chaucer's Canterbury Tales. Try copying the links and loading them in Mirador:
  * The Ellesmere Chaucer, from the Huntingdon Library, California [https://hdl.huntington.org/iiif/2/p15150coll7:2838/manifest.json](https://hdl.huntington.org/iiif/2/p15150coll7:2838/manifest.json)
  * The Hengwrt Chaucer, from the National Library of Wales, Aberystwyth (just copy the section in bold) [https://damsssl.llgc.org.uk/iiif/2.0/4628556/manifest.json?manifest=**https://damsssl.llgc.org.uk/iiif/2.0/4628556/manifest.json**](https://damsssl.llgc.org.uk/iiif/2.0/4628556/manifest.json?manifest=https://damsssl.llgc.org.uk/iiif/2.0/4628556/manifest.json)
  * The Bodmer Chaucer, from Fondation Martin Bodmer, Switzerland [https://www.e-codices.ch/metadata/iiif/fmb-cb-0048/manifest.json](https://www.e-codices.ch/metadata/iiif/fmb-cb-0048/manifest.json)

<figure><img src="../.gitbook/assets/mirador.jpg" alt=""><figcaption><p>Mirador viewer with three manuscripts loaded for comparison</p></figcaption></figure>

* You can navigate and manipulate the images in Mirador in several ways. Clicking and dragging the header or the side of an object allows you to reposition the images in relation to one another. You can zoom in and out using the mouse scroll wheel, and pan around the image by clicking and dragging with the mouse.
* To view the metadata associated with an image, click on the hamburger button (three horizontal lines) to the top left of each object. This will display the metadata in a panel on the left side of the viewer.
* If you want to save or share the current state of the viewer, you can click on the '...' button in the left toolbar. 'Export' generates code that you can copy and send to another user - who can paste it under the 'Import' option in their own browser. You can also save the code for your own use if you want to come back to your workspace at a later date.
