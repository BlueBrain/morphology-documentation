HDF5 Morphology Containers
==========================

For simulations of large regions of a brain using unique, detailed morphologies, the number of morphology files can grow into the millions.
Typical size of each file would be in the kilobyte.
This can be very detrimental to filesystem performance.

HDF5 can be seen as a filesystem inside a single file.
The idea is to copy individual morphology files into subgroups of the container.

Merged HDF5 Morphology Container
--------------------------------

A merged HDF5 morphology container is an HDF5 file.
The top-level a hierarchy of groups one per morphology in the container.
The structure inside these groups is identical to a h5v1 morphology.

The path of each morphology may contain the symbols ``a-zA-Z0-9_.-`` and ``/``.
The ``/`` used to separate subgroups, e.g. the morphology with name ``ae/32/C923`` is stored in a subgroup (``C923``) of a subgroup (``32``) of a top-level group (``ae``).

Recommended HDF5 File Formats
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Performance measurements suggest that a page aggregated file with 4MB pagesize is ideal for GPFS.
