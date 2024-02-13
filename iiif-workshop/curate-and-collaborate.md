---
description: Gather images from multiple objects in one workspace, and share with others
cover: ../.gitbook/assets/biblissima.jpg
coverY: -298
---

# Curate and collaborate

### Exercise: Create and share a Mirador workspace

* Open [Biblissima Portal](https://portail.biblissima.fr/en/) in a new tab. This impressive resource is a library of libraries - a single entry point to access over 650,000 digitised images of manuscripts and books from the 8th-18th centuries, held in 17 different libraries across France.
* Scroll down to open the [Illuminations and marks search tool](https://portail.biblissima.fr/en/bbma.view?vid=search-results\&facet:etype-facet=Illumination\&facet:etype-facet=Mark). From here you can search over 300,000 images by keyword. Biblissima's metadata is largely in French, so try searching for a French noun, e.g. ange (angel), chat (cat), chien (dog), diable (devil), dragon (dragon).
* Scroll through the results to find images with a IIIF logo. Open one in a new tab.
* Note the folio or page number on which the illumination appears, then scroll down to copy the IIIF manifest.
* Go to [Mirador](https://mirador-dev.netlify.app/\_\_tests\_\_/integration/mirador/), and close down any open objects in your workspace by clicking the crosses in the top right corner.
* Click on the 'Start here' button in the top left. Click 'Add resource' in the bottom right to add a new one. Paste your manifest into the text field, and click 'Add'. Click on it to pull it into your workspace.
* You'll notice that Mirador has loaded the whole object, not just the image. In the left hand menu, click the Index icon (it looks like five horizontal lines). This displays a list of all pages in the object. Scroll down until you find the page or folio number that you noted earlier, and click to load it. Zoom into the image.
* Repeat this process a few more times to create a collage based on your chosen keyword.
* When you've finished your collage, click the ellipsis icon in the left hand menu (...). From here, you can export your workspace, allowing you to return to it another day, or share it with others. Mirador is web-based - it isn't downloaded onto your local PC - and it doesn't support user accounts either, so exporting your workspace is the only way to save your work. Clicking the option will generate a long page of code. Copy this, and either email it to yourself, or save in a document.
* If you later want to share your workspace, or return to it to make further edits, find your saved code, and copy it. Open Mirador, and click the ellipsis. This time, choose import workspace, and paste the code. Connections to all the images, on all the pages, in all the manuscripts, from all the different libraries, will be restored, exactly as you left them!

The objects you've loaded to Mirador are not just a collection of images. They're more like a map, that traces paths from those images to their objects and to the repositories in which they were found.

Sharing the workspace achieves more than just sharing a collage of images. The recipient could go to one of the images, and scroll through the rest of the pages in that object, or click a link that would take them to that library's catalogue to see what other manuscripts they hold. IIIF images don’t exist in isolation.

### Bonus exercise: Here's one Biblissima made earlier!

* Open [Biblissima Portal](https://portail.biblissima.fr/en/) in a new tab.
* Scroll down to open the [Iconographic thesaurus](https://portail.biblissima.fr/en/ark:/43093/thb806db559f2abfe3bd6884def6909c7329f5a183). Use the dropdown menus to browse through keywords, e.g. Zoology > Mammals > Horse.
* If there are enough results, Biblissima will generate a huge collage in Mirador. If you chose horses, nearly 5,000 images of horses will be loaded to Mirador. Each image can be clicked on to find out more about the manuscript it belongs to - all the other pages it contains, and all its associated metadata.

Biblissima is a fantastic resource for medieval scholars. But what if the image you want to work with isn't available in IIIF? In the next section, we'll look at how you can create a IIIF manifest with your own images, for free, without requiring any special software or server infrastructure.
