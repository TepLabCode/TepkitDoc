tepkit.io.shengbte.ForceConstants3rd
====================================

.. py:class:: tepkit.io.shengbte.ForceConstants3rd

   Bases: :py:obj:`tepkit.io.StructuredTextFile`



   3rd-order interatomic force constants file in ShengBTE format.



Attributes
----------

.. csv-table::
   :header: "Attribute", "Default Value", "Description"

   "``default_file_name``", "``'FORCE_CONSTANTS_3RD'``", "The default name of file when use ``from_dir()`` ."
   "``df``", "``None``", ""






Methods
-------

.. autoapisummary::

   tepkit.io.shengbte.ForceConstants3rd.from_string
   tepkit.io.shengbte.ForceConstants3rd.calculate_rms
   tepkit.io.shengbte.ForceConstants3rd.calculate_ion_positions
   tepkit.io.shengbte.ForceConstants3rd.calculate_ion_distances




All Members
-----------


.. py:attribute:: default_file_name
   :no-index:
   :value: 'FORCE_CONSTANTS_3RD'


   The default name of file when use ``from_dir()`` .



.. py:attribute:: df
   :no-index:
   :value: None



.. py:method:: from_string(string: str) -> Self
   :no-index:
   :classmethod:


   Parse the string to structured data.



.. py:method:: calculate_rms() -> None
   :no-index:



.. py:method:: calculate_ion_positions(poscar) -> None
   :no-index:


   计算原子在超胞中的位置



.. py:method:: calculate_ion_distances(sposcar) -> pandas.DataFrame
   :no-index:


   计算任意两原子间的距离




