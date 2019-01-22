# GRIX

GRIX is a simple grid system that uses flex to arrange HTML elements.

Listed below are instructions for compiling a *```.scss```* files into a *```.css```* file. In this example, we will compile *```grix.scss```* to *```grix.css```*. The newly compiled CSS file will only include the compressed styling.

## Installation

Include link in the ```<head>``` element.
```
<link href="/css/grix.css" rel="stylesheet">
```
Include ```row``` and ```column``` classes for parent and children elements.
```
<div class="row">
    <div class="col-6">
        <h1>left</h1>
    </div>
    <div class="col-6">
        <h1>right</h1>
    </div>
</div>
```

## Compiler Requirements

 - Download & install [Node.js](https://nodejs.org/en/download/)
 - Install *```node-sass```* via command line: *```npm install -g node-sass```*

## Compiler Instructions

 - How to Manually Compile SCSS to CSS:
   - Open command line within the root folder
   - Run: *```node-sass scss/grix.scss css/grix.css --output-style compressed```*