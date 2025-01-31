---
title: Gallery Perspective
tags: [perspective]
---

import { ProFeature, EntFeature, CenteredImage } from '@site/src/components/CommonBlocks'

<ProFeature />

This perspective offers basic image gallery functionality, like previewing the images from the current folder, a presentation mode in a full screen view.

:::tip
This perspective can only be activated in folder which contains images and photos in the following file formats: JPG, PNG, GIF, BMP, SVG or WEBP.
:::

<CenteredImage
    caption="Showing the regular view of the gallery perspective"
    src="/media/gallery/tagspaces-gallery-overview.png"
    showCaption
  />

## Functionalities in the toolbar

The toolbar of the gallery perspective, located on the top of the previous screenshot, offer the following functionalities:

- **Navigate to parent folder** - opens the parent folder of the current folder.
- **Folder properties** - opens the properties of the current folder.
- **Open previous image** - opens the previous image file from the current folder.
- **Open next image** - opens the next image file in the current folder.
- **Start/stops presentation mode** - toggles on and off the presentation of the images in the current folder, by showing them for 3 seconds. We plan to make this duration configurable in future release.
- **Full screen mode** - opens the currently selected file in full screen mode.
- **File properties** - clicking this button will open the properties of the current file in the regular area for this purpose.
- **Thumbnail bar modes** - clicking this button will toggle through the modes of the thumbnail bar, which are: position on the top, position on the left or hidden. This modes are respected in the full screen mode.
- **Import EXIF/IPTC** - clicking on the button will open the dialog for importing EXIF/IPTC infos from your files.
- **Help** - clicking on the button will open this page.

:::tip
In full screen mode you can navigate through the file by using the left and right key of the keyboard. On a device with touch screen, the image can be changed with the swipe left and right gestures.
:::

## Importing EXIF/IPTC data from JPGs

Many digital cameras are embedding additional information such as geo location in the photos created by them. One common format for this meta data is [EXIF](https://en.wikipedia.org/wiki/Exif). Another format for saving meta data is [IPTC](https://en.wikipedia.org/wiki/IPTC_Information_Interchange_Model), it usually used for embedding keyword and description to JPGs files. The gallery perspective has ability to read and convert the following data into TagSpaces' tags:

- **EXIF geo location** - Takes the latitude and longitude and converts in geo-tags in [Plus Code](https://maps.google.com/pluscodes/) or MGRS format
- **EXIF shooting date and time** - Converts the date and time of the shooting as a date time tag
- **IPTC keywords** - Imports IPTC keywords as regular tags

![Dialog for importing EXIF/IPTC data from JPGs](/media/gallery/import-exif-iptc.png)
