Builder 
===========

###Introduction

Builder is a very simple code merger tool that I use for building/compressing code for medium-large projects.
The tool has three objectives:
- Convert SASS/SCSS to CSS
- Merge many JS / many CSS files into one file (e.g. code.min.js and code.min.css)
- Compress and optimize the code (using Yahoos yui-compiler)

###Scope

The builder is released under the Apache Software License 2.0. Copyright: Malmö City.

The product uses a number of third-party libraries, such as yui compiler etc. These are not included in the sMap product. The copyright of these libraries belongs to their respective authors and are protected by their own license.

The builder package (i.e. the contents of this repository) consists of the builder product on one hand, and the required third-party libraries on the other.

###Requirements

This tool requires:
- Python

Optional:
- [YUI compiler](https://github.com/yui/yuicompressor/releases) for minifying and optimizing the code
- [SASS](http://sass-lang.com/install) for converting SCSS files into CSS files

###Get started

To get started, follow these steps:

1. Clone or download the source code of this repository
2. Download the latest [YUI compiler](https://github.com/yui/yuicompressor/releases)
3. Open the file config_env.json and set the yuiPath to the YUI compiler's location (.jar file)
4. Open the file config_sources.json and add the paths to the files you want to compress
5. Execute the python script build.py using python build.py

This will output 4 files:
- A merged JS file (all JS files merged into one)
- A merged CSS file (all CSS files merged into one)
- A minified JS file (a minified version of the merged JS file)
- A minified CSS file (a minified version of the merged CSS file)

For more options, read below.

###Support

Note that this tool was originally developed for a specific project and might needs some adaptation to fit your needs. I am working on making it more generic and improving the documentation.

###Questions or suggestions?

Contact me at: johan.lahti (at) malmo.se
