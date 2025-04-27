tepkit.io.vasp.eigenval.Eigenval
================================

.. py:class:: tepkit.io.vasp.eigenval.Eigenval

   Bases: :py:obj:`tepkit.io.StructuredTextFile`



   The class of EIGENVAL file for VASP.

   **Refs:**

   - https://www.vasp.at/wiki/index.php/EIGENVAL
   - https://www.vasp.at/wiki/index.php/DOSCAR
   - https://w.vasp.at/forum/viewtopic.php?p=20810
   - https://sisl.readthedocs.io/en/latest/_modules/sisl/io/vasp/eigenval.html



Attributes
----------

.. csv-table::
   :header: "Attribute", "Default Value", "Description"

   "``default_file_name``", "``'EIGENVAL'``", "The default name of file when use ``from_dir()`` ."
   "``data_columns``", "``None``", ""
   "``data``", "``None``", ""
   "``extra_data``", "``None``", ""
   "``df``", "``None``", ""
   "``soc``", "``None``", ""


Properties
----------

.. autoapisummary::

   tepkit.io.vasp.eigenval.Eigenval.index_vbe
   tepkit.io.vasp.eigenval.Eigenval.index_cbe
   tepkit.io.vasp.eigenval.Eigenval.energy_vbm
   tepkit.io.vasp.eigenval.Eigenval.energy_cbm
   tepkit.io.vasp.eigenval.Eigenval.energy_midgap





Methods
-------

.. autoapisummary::

   tepkit.io.vasp.eigenval.Eigenval.from_string
   tepkit.io.vasp.eigenval.Eigenval.get_band




All Members
-----------


.. py:attribute:: default_file_name
   :no-index:
   :value: 'EIGENVAL'


   The default name of file when use ``from_dir()`` .



.. py:attribute:: data_columns
   :no-index:



.. py:attribute:: data
   :no-index:



.. py:attribute:: extra_data
   :no-index:



.. py:attribute:: df
   :no-index:
   :value: None



.. py:attribute:: soc
   :no-index:
   :type:  bool
   :value: None



.. py:method:: from_string(string: str) -> Self
   :no-index:
   :classmethod:


   Parse the string to structured data.



.. py:property:: index_vbe
   :no-index:
   :type: int


   Get the band index of the Valence Band Edge (VBE).
   (Start at 1)



.. py:property:: index_cbe
   :no-index:
   :type: int


   Get the band index of the Conduction Band Edge (VBE).
   (Start at 1)



.. py:property:: energy_vbm
   :no-index:
   :type: float



.. py:property:: energy_cbm
   :no-index:
   :type: float



.. py:property:: energy_midgap
   :no-index:
   :type: float



.. py:method:: get_band(index: str | int)
   :no-index:




