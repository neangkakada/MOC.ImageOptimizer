MOC.ImageOptimizer
==================

Flow package that optimizes generated thumbnail images (jpg, png, gif, svg) for web presentation.

Original files are never affected since copies are always created for thumbnails.

Using jpegtran, optipng, gifsicle and svgo for the optimizations.

Should work with Linux, FreeBSD, OSX, SunOS & Windows (only tested Linux & FreeBSD so far).

Compatible with Flow 3.x

Installation
------------

Requires npm (node.js) to work out of the box, although binaries can also be installed manually without it.

```composer require "moc/imageoptimizer" "~2.0"```

Run `npm install --prefix Resources/Private/Library` in the package (should happen automatically during install).

Configuration
-------------

Using the ``Settings`` configuration, multiple options can be adjusted.

Optimization can be disabled for specific file formats.

Additionally options for optimization level (png & gif), progressive (jpg), pretty (svg) can be adjusted.

Usage of global available binaries can be configured instead or for specific formats.

Usage
_____

Clear thumbnails to generate new ones that will automatically be optimized.

```./flow media:clearthumbnails```