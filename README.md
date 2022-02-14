# Morphology documentation
This repository contains the documentation of the morphology files formats used by Blue Brain. The representations divide into two main topological categories:
* tree-like representation (neurons, astrocytes)
* graph-like representation (vasculature)

To update the documentation, update the rst files located in the source directory.
To update the version number, modify the "version" entry in package.json

## Documentation
morphology-documentation is built and hosted on [readthedocs](https://readthedocs.org/).

* [latest snapshot](http://neurom.readthedocs.org/en/latest/)

To build the documentation locally clone this repository, and run the following command inside it

```tox -e docs```

The documentation is then available under `build/html/index.html`.

Funding & Acknowledgements
-------------------------

The development of this software was supported by funding to the Blue Brain Project, a research center of the École polytechnique fédérale de Lausanne (EPFL), from the Swiss government's ETH Board of the Swiss Federal Institutes of Technology.

Copyright (c) 2022 Blue Brain Project/EPFL
