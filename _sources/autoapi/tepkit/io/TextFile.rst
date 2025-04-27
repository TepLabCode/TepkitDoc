tepkit.io.TextFile
==================

.. py:class:: tepkit.io.TextFile

   Bases: :py:obj:`File`



   The class for text files.
   The base class for `StructuredTextFile` and `TableTextFile` .



Attributes
----------

.. csv-table::
   :header: "Attribute", "Default Value", "Description"

   "``content``", "``None``", "Record the string of the textfile."






Methods
-------

.. autoapisummary::

   tepkit.io.TextFile.from_string
   tepkit.io.TextFile.from_file




All Members
-----------


.. py:attribute:: content
   :no-index:
   :type:  str | None
   :value: None


   Record the string of the textfile.



.. py:method:: from_string(string: str) -> Self
   :no-index:
   :classmethod:


   Save the string to ``self.content`` and return the object.



.. py:method:: from_file(path: tepkit.utils.typing_tools.PathLike) -> Self
   :no-index:
   :classmethod:


   Read the text file, and save its text to self.content.




