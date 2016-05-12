---
title: Coordinate Transformations in ADCIRC.io
tags: 
    - adcirc
    - coordinates
    - camera
---

There seems to be a lot of confusion over how coordinate systems are used in ADCIRC.io, so I'm hoping to clear things up here. I think the easiest way to get a full understanding of how selections work in ADCIRC.io is going to be a step-by-step walkthrough, from reading the data to displaying the mesh to performing a selection. That way I can explain the bits and pieces of various code/libraries/3D concepts that are really necessary, as opposed to trying to learn Javascript/three.js/3D coordinate transformations all separately and then bringing them together. First I'll talk about how the data is read from the fort.14 file and transformed into a coordinate system that can be displayed. Then I'll show how the data is used in three.js to provide interactivity, and finally, I'll show how to get the coordinates (in the mesh's local coordinate system) of a click on screen.

## Preparing an ADCIRC Mesh for Display

The code that calculates the translation and scaling needed to properly display the mesh is found in the /js/files/Fort14.js file. The following code snippet from that file shows the finish_loading() function, which is called once the fort.14 file has been read and the mesh data has been stored in a three.js mesh object.

{% gist b31acc3a79d830612508479f91cd1887 %}