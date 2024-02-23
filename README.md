[![DOI](https://zenodo.org/badge/389640097.svg)](https://zenodo.org/badge/latestdoi/389640097)

# GOESVisualizer

A simple toolbox to retrieve/visualize/save GOES16(east) and GOES17(west) RGB image over a region of interest

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install GOESVisualizer.

```bash
pip install GOESVisualizer
```

## Usage

see example.py

or

```bash
from GOESVisualizer import GSVis

GSobj = GSVis('west', 2021, 7, 20, 12, -125, -117, 35, 45, gamma = 2.5)

```
you have two options here: either make a snapshot for the given time or loop over days/hour;
if you just want a snapshot follow this:

```bash
GSobj.snapshot()

GSobj.savepics()

```

if you are interested in animating a series of images, follow this:

```bash
GSobj.loop(21,4)
GSobj.savepics()
GSobj.animate()

```

Pictures or animated gif will be stored under /pics/


## License
[MIT](https://choosealicense.com/licenses/mit/)
