tepkit.core.symmetry.LayerGroup
===============================

.. py:class:: tepkit.core.symmetry.LayerGroup



Attributes
----------

.. csv-table::
   :header: "Attribute", "Default Value", "Description"

   "``data``", "``None``", ""


Properties
----------

.. autoapisummary::

   tepkit.core.symmetry.LayerGroup.number





Methods
-------

.. autoapisummary::

   tepkit.core.symmetry.LayerGroup.from_file
   tepkit.core.symmetry.LayerGroup.from_poscar
   tepkit.core.symmetry.LayerGroup.get_data_from_spglib
   tepkit.core.symmetry.LayerGroup.add_additional_data




All Members
-----------


.. py:attribute:: data
   :no-index:
   :value: None



.. py:method:: from_file(path, fmt, aperiodic_axis: Axis | Type[Axis] = Axis.a3, sym_prec: float = 1e-05)
   :no-index:
   :classmethod:


   >>> layer_group = LayerGroup.from_file("Bi2Te3.poscar", fmt="vasp")
   >>> layer_group.number
   72
   >>> layer_group.data.international
   'p-3m1'



.. py:method:: from_poscar(poscar: tepkit.io.vasp.Poscar, aperiodic_axis: Axis = Axis.a3, sym_prec: float = 1e-05)
   :no-index:
   :classmethod:



.. py:method:: get_data_from_spglib(cell, aperiodic_axis: Axis = Axis.a3, sym_prec: float = 1e-05)
   :no-index:



.. py:property:: number
   :no-index:
   :type: int



.. py:method:: add_additional_data() -> None
   :no-index:




