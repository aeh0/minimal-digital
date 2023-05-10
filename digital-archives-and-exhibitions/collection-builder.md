---
description: Template-driven digital exhibitions and visualisations
---

# CollectionBuilder

CollectionBuilder is one of a number of static site generators designed specifically for hosting digital exhibitions. Users create a GitHub account, but no coding or command line knowledge is needed to set up or manage the project.

The focus is on metadata, not web design. All users need to do is gather a set of image files, and prepare their associated metadata in a standardised, csv format. CollectionBuilder uses this metadata to conjure an exhibition website according to a pre-programmed template, which can be hosted and served using GitHub Pages. Developed by University of Idaho Library as a tool to create free digital collections, staff soon recognised its equal potential as a teaching tool. It features a gentle learning curve that teaches the principles of good metadata management. Get the metadata right, and the site builds itself.

Being template-based, all sites built using Collection Builder will look the same in terms of layout - the only difference is the digital content supplied, and the functionality, which can scale according to need. A number of visualisation tools are available, as long as the metadata required to drive them is supported.&#x20;

If a user includes subject headings in their metadata, a tag cloud will generate. If dates are included, a timeline will appear. If latitude and longitude data is added, an interactive map will 'pin' the images to geographic locations. The final product gives the impression that a lot of programming has gone into the site, when in fact it is driven solely by csv.

### How to use CollectionBuilder

#### Create a new GitHub repository containing the template code:&#x20;

1. Visit [CollectionBuilder's GitHub Pages repository](https://github.com/CollectionBuilder/collectionbuilder-gh)
2. On the repository home page, click the green 'Use This Template' button (appears on right side above the code area).
3. This brings you to a 'Create a new repository' page. Fill out using these options:
   * Create a lowercase repository name without spaces or special characters. This name will become part of your public site URL
   * Most users should choose 'Public' repository. If you are hosting on GitHub Pages it _must_ be public unless you upgrade to a paid account
   * Leave the 'Include all branches' option unchecked
   * Click on the green button 'Create repository from template'
   * You will be redirected to your new repository!

#### Add your images

Navigate to your repository's **Objects** folders. Delete the demo files. Gather the files you want to use for your project into a single folder on your PC. Consider the following:

* **File formats**. Only jpeg and png images, pdf documents, and mp3 audio are supported.
* **File size.** Unlike Wax, no thumbnails or access derivates will be created - the images loaded will be displayed at their original size. While CollectionBuilder lacks native support for IIIF, jpegs are displayed in a viewer that gives large files a similar zooming effect, though you may notice a slight delay to page load times. File size is therefore a question of balance across the project - you want large enough images to be viewed via zoom, but not too large that they slow the load time, or cause you to exceed GitHub's soft limits on total repository size, somewhere around 1 GB.
* **Filenames.** To avoid issues, use filenames that are unique, lowercase, and feature no spaces or special characters. Underscores (\_) are okay. You will use the exact filenames to populate the 'filename' field of your collection metadata.
* **Do you need to prototype?** CollectionBuilder looks great 'out of the box', but if you plan to spend some time configuring the appearance of your exhibition, consider adding just a few images to your repository in the first instance. If you change so much as a single character of code and want to see how your edit affects the appearance, you will need to 'commit the changes'. Think of this as saving your work. When you commit changes, the entire site will be indexed, which can take several minutes for larger sites. Committing changes will take just seconds if your site is lightweight - you can always add more, or larger, images once the site is set up to your satisfaction.

1. On the home page of your project repository on GitHub, click on the **Objects** folder that appears in the code area of the page
2. Click the **Add file** button and select **Upload files** (appears to right side of page)
3. Click **Choose your files** and navigate to the location of your object files on your PC, and select all the collection items. Or drag and drop all the files from your File Explorer / Finder into the GitHub page. Once the files are uploaded, they will appear listed on the page
4. Scroll down to the **Commit changes** box, write a short commit message in the form, e.g. 'add collection objects', then click the green **Commit changes** button to add them to your repository.

* METADATA
* CONFIG



[Map zoom levels](https://leafletjs.com/examples/zoom-levels/example-delta.html)

#### Enable GitHub Pages:&#x20;

* In your repository, navigate to the **Settings** page (appears on the right along the tabs above the code area): click **Pages** in the left side menu
* Under **Source**, leave the dropdown button as **Deploy from a branch**. Under **Branch** use the dropdown to change from **none** to **main**, then click the **Save** button.
* It will take a few minutes for the build to happen and your site to go live. Refresh the **Pages** page. If the build is successful, an alert will appear near the top providing the URL to your live site. The URL will follow the pattern: **https://username.github.io/repository-name**

For convenience, you might want to copy the URL to display on your repository home page:

1. Go to repository’s home page.
2. On right side of the code area, look for “About” section and click on the cog icon to edit.
3. In the “About” box, paste in your URL, then click “Save”. This will make it easy to access the site in the future!

You can continue to customise the appearance of your site by modifying the HTML, CSS, and JavaScript files that are generated by CollectionBuilder. See the [documentation](https://collectionbuilder.github.io/cb-docs/docs/theme/) for full guidance.

To add new content to your collection, you can add to your metadata spreadsheet and upload new content files to your repository's **Objects** folder. If you make any changes, remember to commit them to update your collection site.

