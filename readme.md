# GRIX

GRIX is a simple grid system that uses CSS Flexbox to dynamically arrange HTML elements.

## Setup

### Basic Layout

Include link in the ```<head>``` element:
```
<link href="css/grix.css" rel="stylesheet">
```
Include ```row``` and ```column``` classes for parent and children elements:
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

### Advanced Layout

To change column widths for mobile views, append ```'-m'``` to the column class:
```
<div class="row">
    <div class="col-3 col-6-m">
        <h1>left</h1>
    </div>
    <div class="col-9 col-6-m">
        <h1>right</h1>
    </div>
</div>
```

## Preprocessor Requirements

 - Download & install [Node.js](https://nodejs.org/en/download/)
 - Install *```node-sass```* via command line: *```npm install -g node-sass```*

## Preprocessor Instructions

Listed below are instructions for compiling a *```.scss```* files into a *```.css```* file. In this example, we will compile *```grix.scss```* to *```grix.css```*. The newly compiled CSS file will only include the compressed styling.

 - How to Manually Compile SCSS to CSS:
   - Open command line within the root folder
   - Run: *```node-sass scss/grix.scss css/grix.css --output-style compressed```*

## Options

GRIX can be customized to match your most unique design layouts. Listed below are various options to use prior to processing to CSS:

 - ```$columns``` - Number of columns. The default value is ```12```.
 - ```$padding``` - Horizontal padding. The default value is ```12px```.
 - ```$mobileWidth``` - Media query width. The default value is ```768px```.
 - ```$columnGrow``` - Column expanding behavior for set widths. The default value is ```true```.