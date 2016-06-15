---
title: The Many Libraries of ADCIRC.io
tags:
    - adcirc
    - development
    - libraries
    - code
---

As I've made my way through the first few months of development of ADCIRC.io, there is one thing that has become abundantly clear: there is a library for just about everything in Javascript. And not just libraries that are used in the code itself, but libraries that are used to help _write_ the code itself. So I thought it might be appropriate at this stage in development, having written some 15,000-odd lines of code thus far, to take a quick step back and take a look at all of the code that I use but _haven't_ written.

# three.js

We'll start off with the library that does most of the heavy lifting in ADCIRC.io, [three.js](http://threejs.org). Three.js is a lightweight 3D library that takes advantage of the ```<canvas>``` element in HTML5, which exposes WebGL functionality. Put more simply, it lets us do really cool 3D visualization within the browser by giving the browser access to your computer's graphics card.

<div id="three_js_geometry_example"></div>

<script src="../assets/js/three/three.min.js"></script>
<script src="../assets/js/three/Detector.js"></script>
<script src="../assets/js/three/geometry_example.js"></script>