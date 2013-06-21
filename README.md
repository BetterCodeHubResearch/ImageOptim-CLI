# ImageOptim-CLI

Automates batch image processing with [ImageOptim](http://imageoptim.com), [ImageAlpha](http://pngmini.com), and [JPEGmini for Mac](http://jpegmini.com/mac) to make lossless optimisation of images part of your automated build process.

If you use [Grunt](http://gruntjs.com) there's also an [ImageOptim-CLI Grunt plugin](https://github.com/JamieMason/grunt-imageoptim).

## Example

    $ imageOptim --directory /path/to/images
    Processing 57 images...
    ✔ Finished in 54 seconds

You can see also a [video screen recording of ImageOptim-CLI](https://www.youtube.com/watch?v=HGBounRIzSs) on YouTube.

## Installation

    $ npm install -g imageoptim-cli

## Usage

    Usage: imageOptim [options]
    
    Options:
    
      -d, --directory     directory of images to process
      -a, --image-alpha   process PNGs with ImageAlpha.app *
      -j, --jpeg-mini     process JPGs with JPEGmini.app **
      -q, --quit          quit ImageOptim.app when complete
      -h, --help          output usage information
      -e, --examples      output usage examples
      -v, --version       output the version number
    
    *  http://pngmini.com
    ** https://itunes.apple.com/us/app/jpegmini/id498944723
    

## Examples

    Examples:
    
    Run ImageAlpha, ImageOptim, JPEGmini, then quit
    $ imageOptim --jpeg-mini --image-alpha --quit --directory path/to/images
    $ imageOptim -j -a -q -d path/to/images
    
    Run ImageOptim only
    $ imageOptim --directory path/to/images
    $ imageOptim -d path/to/images
    

## Credits

ImageOptim-CLI is the work of [Jamie Mason](https://github.com/JamieMason) and [James Stout](https://github.com/jamesstout). It extends [PorneL](https://github.com/pornel)'s brilliant [ImageOptim](https://github.com/pornel/ImageOptim) GUI Application for the Mac.
