
<!-- README.md is generated from README.Rmd. Please edit that file -->
hexwall
=======

The `hexwall.R` file contains one function `gen_hexwall()`, which can be used to generate an image that neatly arranges a folder of hexagons. It makes use of the [ImageMagick](https://www.imagemagick.org/) library via the ROpenSci package [magick](https://github.com/ropensci/magick) to arrange the images.

There are several arguments allowing some control over the function's operation.

-   path: The path to a folder of hexagon stickers (png files are recommended)
-   sticker\_row\_size: The number of stickers in the longest row
-   sticker\_width: The width of each sticker in pixels
-   remove\_small: Should hexagons smaller than the sticker\_width be removed?
-   remove\_size: Should hexagons of an abnormal size be removed?

``` r
source("hexwall.R")
#> Linking to ImageMagick 6.9.7.4
#> Enabled features: fontconfig, freetype, fftw, lcms, pango, x11
#> Disabled features: cairo, ghostscript, rsvg, webp
hexwall("samplehex", sticker_row_size = 3, sticker_width = 200)
```

<img src="README_files/figure-markdown_github/example-1.png" width="600" />

Usage
=====

1.  [Download the repository](https://github.com/mitchelloharawild/hexwall/archive/master.zip)
2.  Unzip and open the R project (`hexwall.Rproj`)
3.  Run `source("hexwall.R")`
4.  Ready to go, use the `hexwall()` function to make your hexagon wall.
