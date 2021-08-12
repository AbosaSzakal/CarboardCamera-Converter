# CarboardCamera-Converter

A slightly modified version of the official Cardboard Camera converter by Google.
The original can be found here: http://storage.googleapis.com/cardboard-camera-converter/index.html

The original limited the output size to 4096x4096 thus heavily reducing the original resolution of the photos.
This version outputs images at their original size, at the cost of increased processing time.

To run it, simply download the repo, open the html and use it as you would the original site.


The changes to the code for future reference:
Set the TARGET_SIZE to 9138 to render a larger image.
Changed the blur mode, because there is a limit of about 5000 to the graphics buffer size.
Currently it downscales the image, blurs it, then resizes back to the larger size before re-rendering the two eye images on top.
The increased time is because of the code used for resizing.
