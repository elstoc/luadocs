---
title: gimp
id: gimp
weight: 140
draft: false
author: "people"
---

## Name

gimp.lua - export and edit with GIMP

## Description

This script provides another storage (export target) for darktable.  Selected
images are exported in the specified format to temporary storage.  GIMP is launched
and opens the files.  After editing, the exported images are overwritten to save the
changes.  When GIMP exits, the exported files are moved into the current collection
and imported into the database.  The imported files then show up grouped with the
originally selected images.

## Usage

* start this script using script manager
* select an image or images for editing with GIMP
* in the export dialog select "Edit with GIMP" and select the format and bit depth for the
  exported image.  Check the  "run_detached" button to run GIMP in detached mode.  Images
  will not be returned to darktable in this mode, but additional images can be sent to 
  GIMP without stopping it.
* Press "export"
* Edit the image with GIMP then save the changes with File->Overwrite....
* Exit GIMP
* The edited image will be imported and grouped with the original image

## Additional Software Required

* GIMP - http://www.gimp.org

## Limitations

* There is no provision for dealing with the xcf files generated by GIMP, since darktable doesn't deal with
  them.  You may want to save the xcf file if you intend on doing further edits to the image or need to save
  the layers used.  Where you save them is up to you.

## Author

Bill Ferguson - wpferguson@gmail.com
