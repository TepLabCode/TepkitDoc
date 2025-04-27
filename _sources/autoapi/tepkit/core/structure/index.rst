tepkit.core.structure
=====================

.. py:module:: tepkit.core.structure


Functions
---------

.. autoapisummary::

   tepkit.core.structure.abc_to_xyz
   tepkit.core.structure.xyz_to_abc


Module Contents
---------------

.. py:function:: abc_to_xyz(abc: NumpyArrayNx3[float], lattice: NumpyArray3x3[float]) -> NumpyArrayNx3[float]

   Usage
   -----
   >>> xyz = abc_to_xyz(abc, lattice)
   >>> xyz = abc_to_xyz(np.column_stack((a, b, c)), b_lattice)
   >>> x, y, z = abc_to_xyz(abc, lattice).T
   >>> x, y, z = abc_to_xyz(np.column_stack((a, b, c)), b_lattice).T


.. py:function:: xyz_to_abc(xyz: NumpyArrayNx3[float], lattice: NumpyArray3x3[float], decimal=15) -> NumpyArrayNx3[float]

   :param xyz: Cartesian coordinates
   :param lattice: Lattice vectors
   :param decimal: Number of decimal places to round to, default is 15 (for float64).
   :return: Fractional coordinates

   Usage
   -----
   >>> abc = xyz_to_abc(xyz, lattice)
   >>> abc = xyz_to_abc(np.column_stack((x, y, z)), lattice)
   >>> a, b, c = xyz_to_abc(xyz, lattice).T
   >>> a, b, c = xyz_to_abc(np.column_stack((x, y, z)), lattice).T


