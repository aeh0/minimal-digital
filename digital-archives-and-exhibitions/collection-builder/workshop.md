---
description: Set up a template digital archive with CollectionBuilder
---

# Workshop

Start by setting up a GitHub account, if you don't have one already.

#### Create a new GitHub repository containing the template code

* Visit [CollectionBuilder's GitHub Pages repository](https://github.com/CollectionBuilder/collectionbuilder-gh)
* On the repository home page, click the green **Use This Template** button (appears on right side above the code area).
* This brings you to a **Create a new repository** page. Fill out using these options:
  * Leave the 'Include all branches' option unchecked
  * Create a lowercase repository name without spaces or special characters. This name will become part of your public site URL
  * Most users should choose **Public** repository. If you are hosting on GitHub Pages it _must_ be public unless you upgrade to a paid account
  * Click on the green button **Create repository**
  * You will be redirected to your new repository!

#### Add your images

Navigate to your repository's **Objects** folders. Delete the demo jpg files if you wish. Gather the files you want to use for your project into a single folder on your PC. Consider the following:

* **File formats**. Only jpeg and png images, pdf documents, and mp3 audio are supported.
* **File size.** Unlike [Wax](../wax.md), no thumbnails or access derivates will be created - all images loaded will be displayed at their original size. While CollectionBuilder lacks native support for IIIF, jpegs are displayed in a viewer that gives large files a similar zooming effect, though you may notice a slight delay to page load times. File size is therefore a question of balance across the project - you want large enough images to be viewed via zoom, but not so large that they slow the load time.&#x20;
* **File quantity.** GitHub has a soft limit on total repository size, around 1 GB, and CollectionBuilder recommends keeping file storage to a 500MB limit for optimal performance. If you want to exceed that, try hosting your images on the Internet Archive. In the filename column of the metadata csv, instead of using the name of the locally hosted file (e.g. LMG000054.jpg), upload the file to the Internet Archive, then paste the direct link to the image file in the filename column. In the case of a jpg, you can find this by clicking on the image, e.g. [https://archive.org/details/LMG00054](https://archive.org/details/LMG00054), when clicked, turns into [https://archive.org/download/LMG00054/LMG00054.jpg](https://archive.org/download/LMG00054/LMG00054.jpg). The site will then pull your images from the Internet Archive, rather than from your objects folder.
* **Filenames.** To avoid issues, use filenames that are unique, lowercase, and feature no spaces or special characters. Underscores (\_) are okay. You will use the exact filenames to populate the 'filename' field of your collection metadata.
* **Do you need to prototype?** CollectionBuilder looks great without any customisation, but if you plan to spend some time configuring the appearance of your exhibition, consider adding just a few images to your repository in the first instance. If you change just a single character of code and want to see how your edit affects the appearance, you will need to 'commit the changes'. Think of this as saving your work. When you commit changes, the entire site will be indexed, which can take several minutes for larger sites. Committing changes will only take a few seconds if your site is lightweight - you can always add more, or larger, images once you're happy with how the site is customised.

1. On the home page of your project repository on GitHub, click on the **Objects** folder that appears in the code area of the page
2. Click the **Add file** button and select **Upload files** (appears to right side of page)
3. Click **Choose your files** and navigate to the location of your object files on your PC, and select all the collection items. Or drag and drop all the files from your File Explorer / Finder into the GitHub page. Once the files are uploaded, they will appear listed on the page
4. Scroll down to the **Commit changes** box, write a short commit message in the form, e.g. 'add collection objects', then click the green **Commit changes** button to add them to your repository.

#### Create and add metadata

Extensive and detailed guidance is provided in the [documentation](https://collectionbuilder.github.io/cb-docs/docs/metadata/gh\_metadata/), including information on [formatting](https://collectionbuilder.github.io/cb-docs/docs/metadata/formatting/). It's recommended to work in Google Sheets in order to avoid encoding errors commonly caused by Microsoft Excel. When you've compiled your metadata according to the documentation, choose the option to Download as Comma-separated values. Give the file a name that uses all lowercase letters, no spaces, and no special characters - don't open it.&#x20;

1. From the home page of your project repository on GitHub, click on the **\_data** folder that appears in the code area of the page
2. Click the **Add file** button and select **Upload files** (appears to right side of page)
3. Click **choose your files**, navigate to the location of the .csv file on your PC, and select it. Or drag the file from your File Explorer / Finder into the GitHub page
4. Scroll down to the **Commit changes** box, write a short commit message in the form, then click the green **Commit changes** button to add the metadata to your repository

#### Configure your site

Next, we need to give Collection Builder information about the site, and where to find the metadata. This is controlled in a file called **config.yml**, which you can access on the main code page of your repository. Click on the filename, then on the pencil icon to the top right to start making edits.

* Essential edits include:

```
title: [The title as it will appear on every page's header and footer]
metadata: [The filename of your metadata .csv file without the extension, e.g. metadata]
```

* Optional edits include:

```
tagline: [An optional descriptive subtitle for the digital collection]
description: [One or two sentences of explanatory text about the collection
   - wrap it in "quotation marks". This description might appear in search 
   result lists, so keep it around 160 characters max]
author: [You! Use your name or GitHub username]
organization-name: [Use to reference your organisation in the site's
   citation, and serve as alternate text for your organisation's logo.
   Wrap in "quotation marks"
organization-link: [URL to your organisation's homepage]
organization-logo-nav: [URL image source for your organisation's logo]
```

* If you don't want to use any of the optional configurations, enter a hash (#) sign at the start of the line to tell the programme to skip over it
* When you've finished editing, scroll down to the **Commit changes** box, write a short commit message in the form, then click the green **Commit changes** button to confirm changes to the site's configuration

#### Enable GitHub Pages

* Finally, we need to be able to view the site!
* In your repository, navigate to the **Settings** page (appears on the right along the tabs above the code area): click **Pages** in the left side menu
* Under **Source**, leave the dropdown button as **Deploy from a branch**. Under **Branch** use the dropdown to change from **none** to **main**, then click the **Save** button.
* It will take a few minutes for the build to happen and your site to go live. Refresh the **Pages** page. If the build is successful, an alert will appear near the top providing the URL to your live site. The URL will follow the pattern: **https://username.github.io/repository-name**

For convenience, you might want to copy the URL to display on your repository home page:

1. Go to your repository’s home page
2. On right side of the code area, look for **About** section and click on the cog icon to edit
3. Check the box next to **Use your GitHub Pages website** then click **Save**. This will make it easy to locate the site in the future

#### Future customisation and changes

You can continue to customise the appearance of your site by modifying the HTML, CSS, and JavaScript files that are generated by CollectionBuilder. See the [documentation](https://collectionbuilder.github.io/cb-docs/docs/theme/) for full guidance.

To add new content to your collection, you can upload new images to your repository's **Objects** folder, and list them in your Google Sheets file, remembering to download and replace the old .csv file in **\_data.** If you make any changes, make sure to **commit** them to update your site.
