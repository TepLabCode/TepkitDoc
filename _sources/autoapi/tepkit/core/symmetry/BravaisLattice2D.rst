tepkit.core.symmetry.BravaisLattice2D
=====================================

.. py:class:: tepkit.core.symmetry.BravaisLattice2D

   Bases: :py:obj:`enum.StrEnum`



   The string enum class for 2D Bravais lattices.

   **Reference:**

   - | International Tables for Crystallography, Vol. E Subperiodic groups
     | —— Kopský, V. (Editor)
     | *Kluwer Academic*, Dordrecht, **2002**.
     | | > Page 6, Table 1.2.1.1

   >>> BravaisLattice2D.mp
   'mp'

   Initialize self.  See help(type(self)) for accurate signature.



Attributes
----------

.. csv-table::
   :header: "Attribute", "Default Value", "Description"

   "``mp``", "``'mp'``", "Oblique"
   "``op``", "``'op'``", "Rectangular"
   "``oc``", "``'oc'``", "Centered-Rectangular"
   "``tp``", "``'tp'``", "Square"
   "``hp``", "``'hp'``", "Hexagonal"


Properties
----------

.. autoapisummary::

   tepkit.core.symmetry.BravaisLattice2D.long_name





Methods
-------

.. autoapisummary::

   tepkit.core.symmetry.BravaisLattice2D.from_string
   tepkit.core.symmetry.BravaisLattice2D.keys
   tepkit.core.symmetry.BravaisLattice2D.to_string
   tepkit.core.symmetry.BravaisLattice2D.differentiate_rectangular_lattice
   tepkit.core.symmetry.BravaisLattice2D.from_bravais_system_2d
   tepkit.core.symmetry.BravaisLattice2D.from_file
   tepkit.core.symmetry.BravaisLattice2D.from_poscar




All Members
-----------


.. py:attribute:: mp
   :no-index:
   :value: 'mp'


   Oblique 



.. py:attribute:: op
   :no-index:
   :value: 'op'


   Rectangular 



.. py:attribute:: oc
   :no-index:
   :value: 'oc'


   Centered-Rectangular 



.. py:attribute:: tp
   :no-index:
   :value: 'tp'


   Square 



.. py:attribute:: hp
   :no-index:
   :value: 'hp'


   Hexagonal 



.. py:method:: from_string(key: str) -> Self
   :no-index:
   :classmethod:


   Get a ``BravaisLattice2D`` instance from a string.

   The string is **case insensitive** and can be any one of the following formats:

   - Short name (``mp``, ...)
   - Long name  (``oblique``, ...)
   - The first three letters of the long name (``obl``, ...)

   :param key: The vaild name of the 2D Bravais Lattice.
   :return: The ``BravaisLattice2D`` instance.



.. py:method:: keys() -> list[str]
   :no-index:
   :classmethod:



.. py:property:: long_name
   :no-index:
   :type: str


   Return the long name of current BravaisLattice2D.



.. py:method:: to_string(style: str) -> str
   :no-index:


    Return the string representation of the current BravaisLattice2D.

   :param style: The style of string representation.

       - ``short``: Short name style.
       - ``long``: Long name style.
       - ``full``: Combined ``<long_name> (<short_name>)`` style,
                   this style should only be used for display.




.. py:method:: differentiate_rectangular_lattice(space_group_number: int) -> Self
   :no-index:
   :classmethod:


   Differentiate a rectangular lattice to ``oc`` or ``op`` based on the number of the space group.

   :param space_group_number: The number of the space group.
   :return: The ``BravaisLattice2D`` instance.
   :raises Exception: If the space group number is not valid for a 2D rectangular lattice.

   **Method:**

   - ``op``:
       - **mP (unique axis c):** 3, 4, 6, 7, 10, 11, 13, 14,
       - **oP:** 16, 17, 18, 19,
              25, 26, 27, 28, 29, 30, 31, 32, 33, 34,
              47, 48, 49, 50, 51, 52, 53, 54, 55, 56, 57, 58, 59, 60, 61, 62,
   - ``oc``:
       - **oS (oC setting):** 20, 21, 35, 36, 37, 38, 39, 40, 41, 63, 64, 65, 66, 67

   **Reference:**

   - | International Tables for Crystallography, Vol. A Space Group Symmetry
     | —— Aroyo, M. I.
     | *Wiley*, **2016**.
     | | > Page 116, Table 1.6.4.5; Page 117–118, Table 1.6.4.7; Page 119, Table 1.6.4.8;





.. py:method:: from_bravais_system_2d(bravais_system_2d: BravaisSystem2D, sg_number=None) -> Self
   :no-index:
   :classmethod:



.. py:method:: from_file(path, fmt, sym_prec=1e-05) -> Self
   :no-index:
   :classmethod:



.. py:method:: from_poscar(poscar, sym_prec=1e-05) -> Self
   :no-index:
   :classmethod:




