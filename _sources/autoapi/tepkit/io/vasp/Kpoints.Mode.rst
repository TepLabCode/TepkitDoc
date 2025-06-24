tepkit.io.vasp.Kpoints.Mode
===========================

.. py:class:: tepkit.io.vasp.Kpoints.Mode

   Bases: :py:obj:`enum.StrEnum`



   The Enum of all supported KPOINTS modes

   Initialize self.  See help(type(self)) for accurate signature.



Attributes
----------

.. csv-table::
   :header: "Attribute", "Default Value", "Description"

   "``Automatic``", "``'Automatic'``", ""
   "``Gamma``", "``'Gamma'``", ""
   "``Monkhorst``", "``'Monkhorst'``", ""
   "``Cartesian``", "``'Cartesian'``", ""
   "``Fractional``", "``'Fractional'``", ""
   "``Line``", "``'Line'``", ""






Methods
-------

.. autoapisummary::

   tepkit.io.vasp.Kpoints.Mode.from_string
   tepkit.io.vasp.Kpoints.Mode.to_pymatgen




All Members
-----------


.. py:attribute:: Automatic
   :no-index:
   :value: 'Automatic'



.. py:attribute:: Gamma
   :no-index:
   :value: 'Gamma'



.. py:attribute:: Monkhorst
   :no-index:
   :value: 'Monkhorst'



.. py:attribute:: Cartesian
   :no-index:
   :value: 'Cartesian'



.. py:attribute:: Fractional
   :no-index:
   :value: 'Fractional'



.. py:attribute:: Line
   :no-index:
   :value: 'Line'



.. py:method:: from_string(string: str) -> Self
   :no-index:
   :classmethod:



.. py:method:: to_pymatgen()
   :no-index:




