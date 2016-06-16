---
title: The Many Libraries of ADCIRC.io
tags:
    - adcirc
    - development
    - libraries
    - code
---

As I've made my way through the first few months of development of ADCIRC.io, there is one thing that has become abundantly clear: there is a library for just about everything in Javascript. And not just libraries that are used in the code itself, but libraries that are used to help _write_ the code itself. So I thought it might be appropriate at this stage in development, having written some 15,000-odd lines of code thus far, to take a quick step back and take a look at all of the code that I use but _haven't_ written.

# The List

First, a list of all of the libraries. Well, two lists, one for libraries ADCIRC.io uses and one for libraries used to create ADCIRC.io. I'll include a little blurb about each one in the following sections talking about what the library is and how it is used in ADCIRC.io.

## Production Libraries

- [Three.js](http://threejs.org)
- [Bootstrap](http://getbootstrap.com/)
- [jQuery](https://jquery.com/)
- [D3](https://d3js.org/)
- [EventDispatcher](https://github.com/mrdoob/eventdispatcher.js)
- [Handlebars](http://handlebarsjs.com/)
- [Lodash](https://lodash.com/)

## Development Libraries

- [Node + npm](https://nodejs.org/en/)
- [Grunt](http://gruntjs.com/)
    - [grunt-bake](https://github.com/MathiasPaumgarten/grunt-bake)
    - [grunt-contrib-concat](https://github.com/gruntjs/grunt-contrib-concat)
    - [grunt-contrib-uglify](https://github.com/gruntjs/grunt-contrib-uglify)
    - [grunt-contrib-jshint](https://github.com/gruntjs/grunt-contrib-jshint)
    - [grunt-contrib-htmlmin](https://github.com/gruntjs/grunt-contrib-htmlmin)
    - [grunt-contrib-watch](https://github.com/gruntjs/grunt-contrib-watch)
    - [grunt-contrib-handlebars](https://github.com/gruntjs/grunt-contrib-handlebars)
- [Handlebars](http://handlebarsjs.com/)


# Three.js

We'll start off with the library that does most of the heavy lifting in ADCIRC.io, [three.js](http://threejs.org). As the name implies, three.js is a lightweight 3D library that takes advantage of the ```<canvas>``` element in HTML5, which exposes WebGL functionality. Put more simply, it lets us do really cool 3D visualization, like the one seen below, within the browser by giving the browser access to your computer's graphics card.

<div id="three_js_geometry_example"></div>

<script src="../assets/js/three/three.min.js"></script>
<script src="../assets/js/three/Detector.js"></script>
<script src="../assets/js/three/geometry_example.js"></script>