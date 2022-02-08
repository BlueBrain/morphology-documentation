.. _glossary:

Glossary
========

.. glossary::

   hdf5
      File format used to store large amounts of scientific data.
      `HDF5 <https://www.hdfgroup.org/HDF5/>`_

   cross section
      A cross section of a cell process at a point is the intersection of that
      cell process with the plane perpendicular to the tangent of
      its longitudinal axis at that point. The actual shape of this
      intersection is not known, so it has to be simplified (see also
      :term:`point` and :term:`perimeter`).

   perimeter
      In a cell process, the perimeter at a point is the perimeter of its
      :term:`cross section`. This is specially necessary for astrocytes because
      the circular approximation for the cross sections can differ greatly from
      the real perimeter and does not suffice for geometrical modelling.

   end-point
      A point with no children. By definition, it has to be the last point in a section.

   neurite
      Either an 'axon', 'basal dendrite', or an 'apical dendrite' type of section.

   point
      A 4-vector composed of floating point numbers.  The first three
      columns represent X, Y, and Z coordinates and the last column represents
      the diameter. Units: micrometers.

   section
      A series of points bounded by any viable combination of branching point (BP),
      root-point (RP), and end-points (EP).
      That is, any of

      * RP-BP
      * BP-BP
      * BP-EP
      * RP-EP.

      A branching point is the boundary between a section and one or more child sections.

      The first point of a section duplicates the last point of its parent, unless the
      parent is a the soma.

   segment
      The shortest representable portion of a neurite.
      A segment is constituted by 2 consecutive points belonging to the same neurite section.

   soma
      The central cell body of a neuron.

   glia endfoot
      A glia process that makes contact with a blood vessel.

   postsynaptic density
      It's a standard neuroscience term. On the postsynaptic side in electron microscope images,
      a blob of dark material that appears to be very dense is seen.


