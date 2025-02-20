# simplify5d

A module for simplifying 2D and 3D lines using Ramer-Douglas-Peucker algorithm.

An extended port of the very fast simplify.js - https://github.com/mourner/simplify-js

## Installation

Install using pip:

```bash
pip install simplify5d
```

## Usage

```python
import numpy as np
from simplify5d import simplify

points_2d = np.array([[0, 0], [1, 1], [2, 2], [3, 3]])
points_3d = np.array([[0, 0, 0], [1, 1, 1], [2, 2, 2], [3, 3, 3]])

simplified_2d = simplify(points_2d, tolerance=1.0, highest_quality=False)
simplified_3d = simplify(points_3d, tolerance=1.0, highest_quality=False)

print("Simplified 2D points:", simplified_2d)
print("Simplified 3D points:", simplified_3d)
