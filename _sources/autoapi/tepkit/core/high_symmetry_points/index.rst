tepkit.core.high_symmetry_points
================================

.. py:module:: tepkit.core.high_symmetry_points


Attributes
----------

.. autoapisummary::

   tepkit.core.high_symmetry_points.high_symmetry_points_2d_tokens


Classes
-------

.. toctree::
   :hidden:

   /autoapi/tepkit/core/high_symmetry_points/HighSymmetryPoints2D

.. autoapisummary::

   tepkit.core.high_symmetry_points.HighSymmetryPoints2D


Functions
---------

.. autoapisummary::

   tepkit.core.high_symmetry_points.get_high_symmetry_points_2d


Module Contents
---------------

.. py:data:: high_symmetry_points_2d_tokens
   :no-index:
   :type:  list[str]


   The unique names of 2D high symmetry points.

   ::

       +---------------------+---------------------+
       | Overview:           |  Right (=90):       |
       | D2  C2B B  C1B D1   |  D2------B------D1  |
       |   C2         C1     |  |       |      |   |
       | C2A            C1A  |  |       |      |   |
       | AR      G      A    |  AR      G------A   |
       | C3A            C4A  |  |              |   |
       |   C3         C4     |  |              |   |
       | D3  C3B BR C4B D4   |  D3------BR-----D4  |
       +---------------------+---------------------+
       | Acute (<90):        |  Obtuse (>90):      |
       |     C2B----B---D1   |  D2---B-----C1B     |
       |   C2      /    |    |  |     \      C1    |
       | C2A      /     |    |  |      \       C1A |
       | AR      G------A    |  AR      G------A   |
       | |              C4A  |  C3A            |   |
       | |            C4     |    C3           |   |
       | D3---BR----C4B      |      C3B----BR--D4  |
       +---------------------+---------------------+


.. py:function:: get_high_symmetry_points_2d(b_lattice: NumpyArray3x3, *, decimal: int = 10, combine: bool = True, split: bool = False) -> pandas.DataFrame

   Get the absolute and relative coordinates of all possible high symmetry points of a 2D material.

   :param b_lattice: The reciprocal lattice of the strcture.
   :param decimal: Used to eliminate minor errors caused by binary. (like 0.9999 or 1e-11)
   :param combine: If True, the dataframe will inclue ["k_abc", "k_xyz"] columns.
   :param split: If True, the dataframe will inclue ["k_a", "k_b", "k_c"] and ["k_x", "k_y", "k_z"] columns.


