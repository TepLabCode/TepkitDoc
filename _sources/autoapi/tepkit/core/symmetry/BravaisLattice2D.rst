tepkit.core.symmetry.BravaisLattice2D
=====================================

.. py:class:: tepkit.core.symmetry.BravaisLattice2D

   Bases: :py:obj:`enum.StrEnum`



   >>> BravaisLattice2D.mp
   'mp'



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



.. py:method:: from_string(key) -> Self
   :no-index:
   :classmethod:



.. py:method:: keys() -> list[str]
   :no-index:
   :classmethod:



.. py:property:: long_name
   :no-index:
   :type: str



.. py:method:: to_string(style) -> str
   :no-index:



.. py:method:: differentiate_rectangular_lattice(space_group_number: int) -> Self
   :no-index:
   :classmethod:



.. py:method:: from_bravais_system_2d(bravais_system_2d: BravaisSystem2D, sg_number=None) -> Self
   :no-index:
   :classmethod:



.. py:method:: from_file(path, fmt, sym_prec=1e-05) -> Self
   :no-index:
   :classmethod:



.. py:method:: from_poscar(poscar, sym_prec=1e-05) -> Self
   :no-index:
   :classmethod:




