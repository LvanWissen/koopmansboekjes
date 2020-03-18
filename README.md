# Koopmansboekjes

| License     |                                                                                                                                                  |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| Source code | [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)                                      |
| Data        | [![License: CC BY-SA 40](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/) |


## Introductie

Collectie 30398, inventarisnummers 1-37 ([https://archief.amsterdam/inventarissen/details/30398](https://archief.amsterdam/inventarissen/details/30398))

## Preprocessing

1. PDFs downloaded from Amsterdam City Archives (see: https://github.com/LvanWissen/saa-scanDownloader)
2. ScanTail (https://scantailor.org/)
3. Tesseract (https://github.com/tesseract-ocr/tesseract). Command: `$ for f in *.tif; do tesseract $f $f -l nld --psm 4 -c preserve_interword_spaces=1; done`

NB: PDFs (inventory numbers 30-37) converted by ImageMagick using `$ for f in *.pdf; do convert -density 600 $f -depth 8 -strip -background white -alpha off $f.tiff; done`

## Contact

[l.vanwissen@uva.nl](mailto:l.vanwissen@uva.nl)







