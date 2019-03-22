## About

The Surfice web page is a way to view 3D meshes using a web browser. While it can view many types of 3D object, it works well with the desktop-based [Surfice](https://www.nitrc.org/projects/surfice/) software. You can export images from Surfice Desktop to Surfice Web, allowing users to view your images on any device - phone, tablet or computer.

[Here is an example of Surfice for Web](https://neurolabusc.github.io/).

## Requirements

You need to have a web server. You simply copy the files from this repository to a folder that will be hosted as a web page. If you do not have a web server, you can make a free [github](https://www.khanacademy.org/computing/computer-programming/html-css/web-development-tools/a/hosting-your-website-on-github) repository that will be shared as a website. If you do use Github, make sure you do not copy this README.md file to you repository (the README file will be shown as a web page instead of the index.html file). An example of a Github-based web server is here [here](https://neurolabusc.github.io/).

## Installation

Simply copy the contents of this repository to a folder that will be displayed on the web. All the required components are included. You may want to edit the config.json file with a text editor to customize your viewer (for example displaying custom meshes).

## Customize

The text file config.js includes a few values that you might want to change. Here are a few of the most relevant ones.

 - "mesh" determines the mesh that will be initially viewed, e.g. "Right.mz3",
 - "overlay" determines whether another mesh will be loaded on top of the first, e.g. "overlay.mz3". Set this to "" if you do not want to load an overlay mesh.
 - "elevation" is the elevation of the camera relative to the mesh in degrees.
 - "azimuth" sets the position of the camera with respect to the mesh.
 - "backColor" determines the back ground color (in hex), for example "#FFFFFF" for white or  "#000000" for black.

## How it works

 - The web viewer requires WebGL 1.0, and uses the [three.js](https://threejs.org/) JavaScript library.
 - Interactive controls are provided by [dat.gui](https://github.com/dataarts/dat.gui).
 - Loading of compressed uses [gunzip.min.js](https://github.com/imaya/zlib.js). Alternatively, [pako](https://github.com/nodeca/pako) will be used if available.


## Alternatives

Surfice for Web provides a simple method for users of the Surfice desktop software to share results. However, there are a lot of great free tools that can do similar work.

 - [brainbrowser](https://github.com/aces/brainbrowser) and includes great [demos](https://brainbrowser.cbrain.mcgill.ca/#demos).
 - [brainR](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4911196/) allows R users to create [interactive web pages](http://bit.ly/1kEJH6q).
 - R users can also try [ggseg](https://github.com/LCBC-UiO/ggseg) which can create [interactive web pages](https://lcbc-uio.github.io/ggseg/articles/ggseg3d.html).
 - [PyCortex](https://www.frontiersin.org/articles/10.3389/fninf.2015.00023/full) helps Python users create [interactive web pages](http://www.gallantlab.org/pycortex/retinotopy_demo/).
 - [mindboggle](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1005350) includes an [open source](https://github.com/binarybottle/roygbiv) project for viewing meshes ([click here for a demo](http://roygbiv.mindboggle.info/roygbiv/web/index.html)).
 - [SOCR Brain Viewer](http://socr.umich.edu/HTML5/BrainViewer/).
 - [Rudolph Pienaar's brain viewer can show tracks](http://www.nmr.mgh.harvard.edu/~rudolph/webgl/brain_viewer/brain_viewer.html) with source provided on [github](https://github.com/danginsburg/webgl-brain-viewer).
 - [Francesco Giorlando's Three.js viewer](https://f.giorlando.org/2014/09/displaying-fmri-images-in-3d-on-the-web-using-three.js/).