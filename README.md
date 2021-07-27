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

GSobj = GSVis('west', 2021, 7, 20, 20, -125, -117, 35, 45, gamma = 1.4)
#
#GSobj = GSVis('east', 2021, 7, 26, 18, -110, -60, 30, 50, gamma = 3)
# only plot
GSobj.plotGS()
# or only save
GSobj.plotGS(True,'sample.png')

```

## License
[MIT](https://choosealicense.com/licenses/mit/)
