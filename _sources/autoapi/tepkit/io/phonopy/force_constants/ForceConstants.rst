tepkit.io.phonopy.force_constants.ForceConstants
================================================

.. py:class:: tepkit.io.phonopy.force_constants.ForceConstants

   Bases: :py:obj:`tepkit.io.StructuredTextFile`



   2nd-order interatomic force constants file in Phonopy format.



Attributes
----------

.. csv-table::
   :header: "Attribute", "Default Value", "Description"

   "``default_file_name``", "``'FORCE_CONSTANTS'``", "The default name of file when use ``from_dir()`` ."
   "``df``", "``None``", ""






Methods
-------

.. autoapisummary::

   tepkit.io.phonopy.force_constants.ForceConstants.from_string




All Members
-----------


.. py:attribute:: default_file_name
   :no-index:
   :value: 'FORCE_CONSTANTS'


   The default name of file when use ``from_dir()`` .



.. py:attribute:: df
   :no-index:
   :value: None



.. py:method:: from_string(string: str) -> Self
   :no-index:
   :classmethod:


   Parse the string to structured data.




