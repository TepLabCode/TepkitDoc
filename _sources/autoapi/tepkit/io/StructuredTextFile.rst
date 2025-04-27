tepkit.io.StructuredTextFile
============================

.. py:class:: tepkit.io.StructuredTextFile

   Bases: :py:obj:`TextFile`



   The class for text file with special structure.




Properties
----------

.. autoapisummary::

   tepkit.io.StructuredTextFile.lines





Methods
-------

.. autoapisummary::

   tepkit.io.StructuredTextFile.from_string
   tepkit.io.StructuredTextFile.from_file
   tepkit.io.StructuredTextFile.to_file




All Members
-----------


.. py:method:: from_string(string: str) -> Self
   :no-index:
   :classmethod:


   Parse the string to structured data.



.. py:method:: from_file(path: tepkit.utils.typing_tools.PathLike) -> Self
   :no-index:
   :classmethod:


   从文件中读取文本，然后调用 from_string 读取数据。



.. py:property:: lines
   :no-index:



.. py:method:: to_file(path) -> None
   :no-index:


   Write the data of the object to a file.




