# Missing Data

The notebook checks missing values early with `isnull().sum()`.

Keeping the check near the start helps avoid training a model on unexpected nulls or silently losing rows during transformations.

