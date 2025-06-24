tepkit.io.TableTextFile
=======================

.. py:class:: tepkit.io.TableTextFile

   Bases: :py:obj:`TextFile`



   The class for text files.
   The base class for `StructuredTextFile` and `TableTextFile` .



Attributes
----------

.. csv-table::
   :header: "Attribute", "Default Value", "Description"

   "``default_from_file_config``", "``None``", ""
   "``column_indices``", "``None``", ""
   "``column_indices_autofill``", "``None``", ""
   "``df``", "``None``", ""






Methods
-------

.. autoapisummary::

   tepkit.io.TableTextFile.from_file




All Members
-----------


.. py:attribute:: default_from_file_config
   :no-index:



.. py:attribute:: column_indices
   :no-index:
   :type:  dict



.. py:attribute:: column_indices_autofill
   :no-index:
   :type:  dict



.. py:attribute:: df
   :no-index:
   :type:  pandas.DataFrame | None
   :value: None



.. py:method:: from_file(path: tepkit.utils.typing_tools.PathLike = None)
   :no-index:
   :classmethod:


   Read the text file, and save its text to self.content.




