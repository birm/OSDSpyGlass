# OSDSpyGlass
A Customizable Spyglass Which Follows the Mouse, for OpenSeaDragon

## Initialization
This tool requires that OpenSeaDragon is initialized twice; once for the base image, and once for the spyglass. The spyglass should be in its own div.

Since it's a good idea to wait for OpenSeaDragon to finish its initialization before initializing the magnifier, the spyglass tool returns a function, intended to be used like ```window.setTimeout(Spyglass(viewer, spyglass_viewer),500);```.

The arguments to Spyglass are the OpenSeaDragon objects for the base image and spyglass, respectively.

To toggle visible, I recommend a style rule tied to a class, and toggle it using ```modal_viewer.classList.toggle("invisible")```.

## Usage
Zoom is set as an attribute on the spyglass's div in the html document, called 'zoomlevel'. It defaults to the max zoom if not otherwise set.

The height, width, and style of the spyglass are set by changing the style of the spyglass's div.
