# GRIX

GRIX is a simple grid system that uses CSS Flexbox to dynamically arrange HTML elements.

[DEMO](https://raw.githack.com/doppl3r/grix/master/index.html)

## Setup

### Basic Layout

Include link in the ```<head>``` element:
```
<link href="css/grix.css" rel="stylesheet">
```
Include ```row``` and ```column``` classes for parent and children elements

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

**Optional**: You can use a default column if you prefer to use a generic list of equal columns. Ex:  ```class="col"```

### Advanced Layout

To change column widths for mobile views, append ```-m``` to a column class:
```
<div class="row">
    <div class="col-6 col-4-m">
        <h1>left</h1>
    </div>
    <div class="col-6 col-8-m">
        <h1>right</h1>
    </div>
</div>
```

**Optional**: You can force a width on both views by only using the ```-m``` class. Ex: ```class="col-4-m"```

## Preprocessor Requirements

 - Download & install [Node.js](https://nodejs.org/en/download/)
 - Install *```node-sass```* via command line: *```npm install -g node-sass```*

## Preprocessor Instructions

Listed below are instructions for compiling a *```.scss```* files into a *```.css```* file. In this example, we will compile *```grix.scss```* to *```grix.css```*. The newly compiled CSS file will only include the compressed styling.

 - How to Manually Compile SCSS to CSS:
   - Open command line within the root folder
   - Run: *```node-sass scss/grix.scss css/grix.css --output-style compressed```*

## Preprocessor Options

GRIX can be customized to match your most unique design layouts. Listed below are various preprocessor options:

 - ```$columns``` - Number of columns. The default number value is ```12```
 - ```$padding``` - Horizontal padding. The default string value is ```12px```
 - ```$mobileWidth``` - Media query width. The default string value is ```768px```
 - ```$columnGrow``` - Column expanding behavior for set widths. The default boolean value is ```true```
 - ```$suffix``` - Media query suffix. The default string value is ```-m```