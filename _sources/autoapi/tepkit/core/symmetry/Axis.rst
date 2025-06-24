tepkit.core.symmetry.Axis
=========================

.. py:class:: tepkit.core.symmetry.Axis

   Bases: :py:obj:`int`, :py:obj:`enum.Enum`



   The int enum class for the base vectors of a :math:`ℝ^3` space.

   >>> vector = (3.1, 4.1, 5.9)
   >>> vector[Axis.a1]
   3.1
   >>> vector[Axis.a2]
   4.1
   >>> vector[Axis.a3]
   5.9

   Initialize self.  See help(type(self)) for accurate signature.



Attributes
----------

.. csv-table::
   :header: "Attribute", "Default Value", "Description"

   "``a1``", "``0``", ""
   "``a2``", "``1``", ""
   "``a3``", "``2``", ""









All Members
-----------


.. py:attribute:: a1
   :no-index:
   :value: 0



.. py:attribute:: a2
   :no-index:
   :value: 1



.. py:attribute:: a3
   :no-index:
   :value: 2




